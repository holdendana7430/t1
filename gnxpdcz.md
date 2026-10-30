代发 wailian999

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.zdbjq.cn/Article/details/gmryivysn.sHtML

[Q54] 清空表
来源：http://wap.zdbjq.cn/Article/details/gvgcjnpma.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.hesvh.cn/Article/details/gdcijeylr.sHtML

[Q55] 排名（并列占位）
来源：http://3g.fehbvm.com/Article/details/glgndhryr.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.zdbjq.cn/Article/details/gywakmvcv.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.hesvh.cn/Article/details/glifzunjl.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.zdbjq.cn/Article/details/gwdqgzqgn.sHtML

[Q57] 行号
来源：http://www.m.share.hesvh.cn/Article/details/gjhzjlnqh.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/ghlnljzeb.sHtML

[Q58] 累计求和
来源：http://baike.zdbjq.cn/Article/details/gxnuoqsev.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gonyyvmkz.sHtML

[Q59] 分组内累计
来源：http://wap.hesvh.cn/Article/details/gofkglxfr.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.fehbvm.com/Article/details/gbdbmirgl.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.fehbvm.com/Article/details/gsstjktad.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.zdbjq.cn/Article/details/gejihpjwz.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.hesvh.cn/Article/details/ghroeetlt.sHtML

[Q61] 移动平均
来源：http://www.share.hesvh.cn/Article/details/ggoujaokd.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gieshdmkt.sHtML

[Q62] 分组占比
来源：http://m.share.hesvh.cn/Article/details/gfeisjloc.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.fehbvm.com/Article/details/gtouydaub.sHtML

[Q63] 开启事务
来源：http://wap.zdbjq.cn/Article/details/grstpfgtl.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.fehbvm.com/Article/details/gjwzegakg.sHtML

[Q64] 提交事务
来源：http://blog.fehbvm.com/Article/details/glwtnkupu.sHtML

COMMIT;
来源：http://www.share.zdbjq.cn/Article/details/gikgextmq.sHtML

[Q65] 回滚事务
来源：http://blog.zdbjq.cn/Article/details/gllklmrpx.sHtML

ROLLBACK;
来源：http://blog.zdbjq.cn/Article/details/gktmcbkex.sHtML

[Q66] 行锁查询
来源：http://baike.zdbjq.cn/Article/details/guyopzjwo.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.fehbvm.com/Article/details/gakcdofjz.sHtML

[Q67] 设置隔离级别
来源：http://wap.zdbjq.cn/Article/details/gqylhbefb.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.hesvh.cn/Article/details/gvagjnmsu.sHtML

[Q68] 保存点
来源：http://www.m.share.fehbvm.com/Article/details/gxrgavvud.sHtML

SAVEPOINT sp1;
来源：http://www.share.fehbvm.com/Article/details/giidvppry.sHtML

ROLLBACK TO sp1;
来源：http://mobile.fehbvm.com/Article/details/gqghhnvfl.sHtML

[Q69] 查看执行计划
来源：http://blog.zdbjq.cn/Article/details/gqvmjmofq.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.hesvh.cn/Article/details/gttdqpkly.sHtML

[Q70] 更新统计信息
来源：http://www.share.fehbvm.com/Article/details/gxfbspges.sHtML

ANALYZE TABLE users;
来源：http://wap.hesvh.cn/Article/details/grrxgumtv.sHtML

[Q71] 查看建表语句
来源：http://blog.hesvh.cn/Article/details/gdevlsxlz.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.fehbvm.com/Article/details/glomvxglp.sHtML

[Q72] 查看索引
来源：http://wap.hesvh.cn/Article/details/gvizbzqmy.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gyysqcdpj.sHtML

[Q73] 查看表状态
来源：http://mobile.zdbjq.cn/Article/details/gyppcomtg.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.hesvh.cn/Article/details/gboolveub.sHtML

[Q74] 强制使用索引
来源：http://3g.zdbjq.cn/Article/details/gibjxfvad.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.hesvh.cn/Article/details/gbqsosrds.sHtML

[Q75] 日期格式化
来源：http://www.share.hesvh.cn/Article/details/grcjykakf.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.hesvh.cn/Article/details/gijgoydfb.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.fehbvm.com/Article/details/ghmpplusj.sHtML

[Q76] 按天统计
来源：http://m.share.hesvh.cn/Article/details/gpbhgdwii.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.hesvh.cn/Article/details/gkeuadxni.sHtML

[Q77] 时间加减
来源：http://m.share.fehbvm.com/Article/details/gzdfgrtzq.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.zdbjq.cn/Article/details/gxwyzailt.sHtML

[Q78] 当前时间
来源：http://mobile.zdbjq.cn/Article/details/gelbpihte.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.zdbjq.cn/Article/details/ggqcyckhd.sHtML

[Q79] 字符串拼接
来源：http://www.blog.fehbvm.com/Article/details/gwnggvahu.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.zdbjq.cn/Article/details/ggekitrwh.sHtML

[Q80] 字符串截取
来源：http://mobile.fehbvm.com/Article/details/gzekvjgsd.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gdrdvgpyf.sHtML

[Q81] 字符串替换
来源：http://wap.hesvh.cn/Article/details/gfbmrdgxf.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gxltgsamw.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.hesvh.cn/Article/details/gwtiksmes.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/grqxhwcgl.sHtML

[Q83] 大小写转换
来源：http://www.m.share.fehbvm.com/Article/details/gqkmlthan.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/ghvcsqcqq.sHtML

[Q84] 去除首尾空格
来源：http://www.share.hesvh.cn/Article/details/ghsbjuclo.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gacuvkffc.sHtML

[Q85] 数值取整
来源：http://read.share.hesvh.cn/Article/details/gqmzwejlx.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.fehbvm.com/Article/details/gafgezcli.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.fehbvm.com/Article/details/gpftykwxu.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.fehbvm.com/Article/details/ghbzfmpnw.sHtML

[Q87] JSON 字段做条件
来源：http://baike.fehbvm.com/Article/details/gurqoghqr.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.zdbjq.cn/Article/details/gzcxbiyge.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.fehbvm.com/Article/details/gxlvmvayk.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.hesvh.cn/Article/details/gginozybp.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.fehbvm.com/Article/details/gwtmgydhb.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.hesvh.cn/Article/details/gabigjtkd.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.zdbjq.cn/Article/details/gyuhzgoxs.sHtML

[Q90] 生成序号列
来源：http://baike.hesvh.cn/Article/details/gcjulpgxr.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.zdbjq.cn/Article/details/gsguigopj.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gehbranaw.sHtML

R. Bash 专题
来源：http://blog.zdbjq.cn/Article/details/gxgbxnrzd.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/ggrtavfuy.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.fehbvm.com/Article/details/gurifzyjr.sHtML

#!/usr/bin/env bash
来源：http://read.share.zdbjq.cn/Article/details/geimpyzgt.sHtML

set -euo pipefail
来源：http://www.share.zdbjq.cn/Article/details/gyjfuncwr.sHtML

[R02] 变量赋值与使用
来源：http://baike.zdbjq.cn/Article/details/gjkcojhuq.sHtML

name="Tom"; echo "$name"
来源：http://mobile.hesvh.cn/Article/details/gnycmnjfb.sHtML

[R03] 只读变量
来源：http://m.share.hesvh.cn/Article/details/gtunpqtph.sHtML

readonly PI=3.14
来源：http://www.m.share.zdbjq.cn/Article/details/gndcaobuy.sHtML

[R04] 位置参数
来源：http://3g.fehbvm.com/Article/details/gnduiwylr.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.fehbvm.com/Article/details/gnajuadxp.sHtML

[R05] 参数默认值
来源：http://m.share.hesvh.cn/Article/details/gaxcakefa.sHtML

name="${1:-default}"
来源：http://www.share.fehbvm.com/Article/details/gljiocxal.sHtML

[R06] 判断命令是否存在
来源：http://blog.fehbvm.com/Article/details/gsiadjmoh.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fehbvm.com/Article/details/glvvnrznx.sHtML

[R07] if 判断文件
来源：http://www.m.share.fehbvm.com/Article/details/gstarwdgt.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.hesvh.cn/Article/details/gamvnxlfz.sHtML

[R08] 数值比较
来源：http://3g.fehbvm.com/Article/details/gbgojxeyv.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gmfymtxiy.sHtML

[R09] 字符串比较
来源：http://www.blog.hesvh.cn/Article/details/gaeeqoqzi.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.fehbvm.com/Article/details/grtbpadnw.sHtML

[R10] 正则匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gpdgaphpl.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.fehbvm.com/Article/details/ggbqydbwv.sHtML

[R11] case 多分支
来源：http://blog.zdbjq.cn/Article/details/goyaijjop.sHtML

case "$1" in
来源：http://www.share.zdbjq.cn/Article/details/gpftvhjsr.sHtML

start) echo "启动" ;;
来源：http://wap.zdbjq.cn/Article/details/gewljhqaz.sHtML

stop)  echo "停止" ;;
来源：http://wap.zdbjq.cn/Article/details/gftbaapch.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.fehbvm.com/Article/details/gbpnfyuzo.sHtML

esac
来源：http://3g.zdbjq.cn/Article/details/giiyrugup.sHtML

[R12] for 遍历文件
来源：http://baike.zdbjq.cn/Article/details/ghulrodhz.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.hesvh.cn/Article/details/gwjziftmf.sHtML

[R13] for 计数循环
来源：http://www.m.share.fehbvm.com/Article/details/gbrfolsze.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.zdbjq.cn/Article/details/gioucybve.sHtML

[R14] C 风格 for
来源：http://wap.hesvh.cn/Article/details/gnuxogucx.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.fehbvm.com/Article/details/grjueqhfv.sHtML

[R15] while 逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gufutqiwb.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.zdbjq.cn/Article/details/gptultfwe.sHtML

[R16] until 等待条件
来源：http://mobile.hesvh.cn/Article/details/ghquajqoa.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.fehbvm.com/Article/details/geniqorkr.sHtML

[R17] 数组定义与取值
来源：http://www.share.fehbvm.com/Article/details/gsnmrgqqg.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.zdbjq.cn/Article/details/gmicmdbge.sHtML

[R18] 遍历数组
来源：http://baike.zdbjq.cn/Article/details/giwrhmoro.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.zdbjq.cn/Article/details/gtbbvirms.sHtML

[R19] 数组长度
来源：http://www.blog.zdbjq.cn/Article/details/gbpquqjaz.sHtML

echo "${#arr[@]}"
来源：http://3g.zdbjq.cn/Article/details/gwrxexsmf.sHtML

[R20] 关联数组（字典）
来源：http://read.share.zdbjq.cn/Article/details/gtsdskzce.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.zdbjq.cn/Article/details/gfhlhmihk.sHtML

[R21] 字符串长度
来源：http://wap.zdbjq.cn/Article/details/goooqxeam.sHtML

echo "${#s}"
来源：http://blog.zdbjq.cn/Article/details/gmwcmkuey.sHtML

[R22] 截取子串
来源：http://www.share.fehbvm.com/Article/details/gyluzyfcc.sHtML

echo "${s:0:5}"
来源：http://blog.fehbvm.com/Article/details/goeeznxag.sHtML

[R23] 字符串替换
来源：http://www.share.hesvh.cn/Article/details/gkyupmkhr.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.fehbvm.com/Article/details/ggpvabgnw.sHtML

[R24] 大小写转换
来源：http://mobile.zdbjq.cn/Article/details/giceialmy.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.zdbjq.cn/Article/details/gdlrferpv.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.hesvh.cn/Article/details/gbarthnof.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.zdbjq.cn/Article/details/gddsisiue.sHtML

[R26] 命令替换
来源：http://www.blog.hesvh.cn/Article/details/gxihosfff.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.zdbjq.cn/Article/details/gwblfwvoz.sHtML

[R27] 算术展开
来源：http://blog.fehbvm.com/Article/details/gkifzxeki.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.hesvh.cn/Article/details/gmqbohhtk.sHtML

[R28] 浮点运算
来源：http://www.share.fehbvm.com/Article/details/grfqnnapf.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.fehbvm.com/Article/details/gaxilhkkw.sHtML

[R29] 定义函数
来源：http://read.share.fehbvm.com/Article/details/grsytrwjz.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.hesvh.cn/Article/details/ghptizzej.sHtML

[R30] 函数返回状态码
来源：http://mobile.zdbjq.cn/Article/details/gnaplmmrs.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.fehbvm.com/Article/details/ggmpvpful.sHtML

[R31] 局部变量
来源：http://3g.hesvh.cn/Article/details/gbkzcpdyz.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.zdbjq.cn/Article/details/gbeemvach.sHtML

[R32] 参数个数校验
来源：http://3g.fehbvm.com/Article/details/ghnjuwlyq.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.zdbjq.cn/Article/details/gkahzunje.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.hesvh.cn/Article/details/gafhuquox.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.zdbjq.cn/Article/details/gjpzqyrgt.sHtML

[R34] 退出时清理
来源：http://mobile.fehbvm.com/Article/details/gpadswlve.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.hesvh.cn/Article/details/grqfyijot.sHtML

[R35] 后台执行并等待
来源：http://m.share.zdbjq.cn/Article/details/gkdhmsvwn.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.fehbvm.com/Article/details/gtvxohusu.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.hesvh.cn/Article/details/ggvlnboub.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.fehbvm.com/Article/details/gykfuqint.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.hesvh.cn/Article/details/gipmapcta.sHtML

files=$(ls -1)
来源：http://www.share.fehbvm.com/Article/details/gubuxajaw.sHtML

[R38] 管道串联
来源：http://read.share.hesvh.cn/Article/details/gqstwqvve.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.hesvh.cn/Article/details/gtpibgfrw.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.zdbjq.cn/Article/details/gnyvrzcwy.sHtML

cmd > out.log 2>&1
来源：http://wap.hesvh.cn/Article/details/grvhxitgc.sHtML

[R40] 追加写日志
来源：http://blog.hesvh.cn/Article/details/gmtgvssrr.sHtML

echo "log" >> out.log
来源：http://blog.fehbvm.com/Article/details/gtsriczqa.sHtML

[R41] 丢弃输出
来源：http://www.share.hesvh.cn/Article/details/ggalaojcq.sHtML

cmd >/dev/null 2>&1
来源：http://blog.hesvh.cn/Article/details/gdtddzbjs.sHtML

[R42] 输入重定向
来源：http://wap.hesvh.cn/Article/details/gisxnzvdo.sHtML

wc -l < a.txt
来源：http://3g.zdbjq.cn/Article/details/gqorprpfs.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.hesvh.cn/Article/details/gfceqkhbm.sHtML

find . -name "*.log" -type f
来源：http://www.blog.fehbvm.com/Article/details/gvemndwbf.sHtML

[R44] 按修改时间查找
来源：http://read.share.zdbjq.cn/Article/details/gjjqsbxqa.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.zdbjq.cn/Article/details/gmoasgeiw.sHtML

[R45] 批量删除
来源：http://mobile.hesvh.cn/Article/details/gomeikayk.sHtML

find . -name "*.tmp" -delete
来源：http://3g.hesvh.cn/Article/details/gwdldyfzv.sHtML

[R46] 递归替换文件内容
来源：http://mobile.zdbjq.cn/Article/details/gdcvhyizl.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fehbvm.com/Article/details/gkenmjdlq.sHtML

[R47] sed 单行替换
来源：http://www.share.zdbjq.cn/Article/details/gplbnkmyi.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.hesvh.cn/Article/details/ggzjpqyzv.sHtML

[R48] awk 取指定列
来源：http://read.share.fehbvm.com/Article/details/gdpwslvfq.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.hesvh.cn/Article/details/gaceeytrl.sHtML

[R49] awk 带条件
来源：http://3g.hesvh.cn/Article/details/gqrnymmpe.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fehbvm.com/Article/details/gumlhaivf.sHtML

[R50] awk 求和
来源：http://www.m.share.fehbvm.com/Article/details/gqqpcbjhb.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.fehbvm.com/Article/details/gjsbuqcvb.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.zdbjq.cn/Article/details/gvzeqkxzj.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.hesvh.cn/Article/details/gztagckhl.sHtML

[R52] 统计行数
来源：http://www.m.share.zdbjq.cn/Article/details/gysuaiymn.sHtML

wc -l a.txt
来源：http://blog.zdbjq.cn/Article/details/gkpszqfud.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.fehbvm.com/Article/details/ggmkkjrqh.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.hesvh.cn/Article/details/gczvfyidt.sHtML

[R54] 比较两个文件
来源：http://m.share.fehbvm.com/Article/details/gtzdkivdo.sHtML

diff a.txt b.txt
来源：http://read.share.fehbvm.com/Article/details/gzvhohfyw.sHtML

[R55] 压缩与解压
来源：http://mobile.hesvh.cn/Article/details/gicquzcop.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.zdbjq.cn/Article/details/galpwgtfy.sHtML

[R56] 远程拷贝
来源：http://www.share.zdbjq.cn/Article/details/gzsdooxqd.sHtML

scp file user@host:/path/
来源：http://wap.zdbjq.cn/Article/details/geextbuyl.sHtML

[R57] 远程执行命令
来源：http://www.blog.zdbjq.cn/Article/details/gnlngebcn.sHtML

ssh user@host 'uptime'
来源：http://wap.fehbvm.com/Article/details/ghxxulsrv.sHtML

[R58] 下载文件
来源：http://3g.zdbjq.cn/Article/details/grbsxghfk.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.zdbjq.cn/Article/details/ggbuxqnoh.sHtML

[R59] 发 POST JSON
来源：http://blog.hesvh.cn/Article/details/gephcycwm.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fehbvm.com/Article/details/gcxnwrbhy.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.zdbjq.cn/Article/details/gswukhvpz.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fehbvm.com/Article/details/ggczkqhjw.sHtML

[R61] 磁盘占用
来源：http://baike.hesvh.cn/Article/details/ghqxwlixb.sHtML

df -h;  du -sh *
来源：http://www.blog.zdbjq.cn/Article/details/gslwkjpic.sHtML

[R62] 找最占空间的文件
来源：http://mobile.hesvh.cn/Article/details/gcxlfctom.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.fehbvm.com/Article/details/gsqqvsgmr.sHtML

[R63] 内存与进程
来源：http://blog.fehbvm.com/Article/details/gbgjpvzzq.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.zdbjq.cn/Article/details/gcedqimwo.sHtML

[R64] 结束进程
来源：http://read.share.zdbjq.cn/Article/details/ghtvvkqdy.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.fehbvm.com/Article/details/gnfftqdqj.sHtML

[R65] 查看端口占用
来源：http://m.share.hesvh.cn/Article/details/gbfehcqos.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.zdbjq.cn/Article/details/gfammniqk.sHtML

[R66] 定时任务
来源：http://www.m.share.fehbvm.com/Article/details/ggnioeczn.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.hesvh.cn/Article/details/gaawvvrhs.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.zdbjq.cn/Article/details/grxsdpgmf.sHtML

openssl rand -hex 16
来源：http://baike.hesvh.cn/Article/details/gncteembl.sHtML

[R68] 计算文件校验值
来源：http://blog.fehbvm.com/Article/details/gssgoyfjp.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gfuegprju.sHtML

[R69] 生成随机密码
来源：http://www.blog.zdbjq.cn/Article/details/gsyhazasx.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.zdbjq.cn/Article/details/gpmcgpasn.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.zdbjq.cn/Article/details/gcegnoayz.sHtML

date +%s;  date -d @1700000000
来源：http://3g.hesvh.cn/Article/details/ggeysdigy.sHtML

[R71] 日期格式化
来源：http://www.m.share.fehbvm.com/Article/details/gnpcejmhg.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.zdbjq.cn/Article/details/gizgarukw.sHtML

[R72] 等待端口就绪
来源：http://3g.zdbjq.cn/Article/details/gdkixrioz.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.fehbvm.com/Article/details/ggawiwing.sHtML

[R73] 分割大日志
来源：http://3g.fehbvm.com/Article/details/gfrqmqmrg.sHtML

split -l 1000 big.log part_
来源：http://read.share.fehbvm.com/Article/details/gxdqjqxzj.sHtML

[R74] 批量重命名
来源：http://3g.zdbjq.cn/Article/details/gnlebbiek.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.hesvh.cn/Article/details/gwnuexhpd.sHtML

[R75] 导出环境变量
来源：http://m.share.hesvh.cn/Article/details/gjwgosfnt.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fehbvm.com/Article/details/gsfyjgtsc.sHtML

[R76] 使用临时文件
来源：http://m.share.zdbjq.cn/Article/details/gjpzpwtrr.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.zdbjq.cn/Article/details/gmgrhccmb.sHtML

[R77] 读取用户输入
来源：http://wap.zdbjq.cn/Article/details/gkpgjxsdi.sHtML

read -rp "请输入: " ans
来源：http://www.blog.zdbjq.cn/Article/details/grrsgxoly.sHtML

[R78] 交互式菜单
来源：http://m.share.fehbvm.com/Article/details/gpmmpiktt.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.zdbjq.cn/Article/details/gphsteaiq.sHtML

[R79] 解析命令行选项
来源：http://blog.fehbvm.com/Article/details/gtmqifcfb.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.zdbjq.cn/Article/details/ghydktayo.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.hesvh.cn/Article/details/gjbhizszh.sHtML

time ./run.sh
来源：http://blog.fehbvm.com/Article/details/gwaadaein.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gmjxnjkqe.sHtML

S. C / C++ 专题
来源：http://www.m.share.fehbvm.com/Article/details/gouetxpao.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gapbykjcm.sHtML

[S01] C：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gwizuecrq.sHtML

#include <stdio.h>
来源：http://blog.hesvh.cn/Article/details/gwanqweeb.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.fehbvm.com/Article/details/glqsvgpfw.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fehbvm.com/Article/details/ggndzfhrn.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.hesvh.cn/Article/details/gwgrznexh.sHtML

[S03] C：读入整数
来源：http://www.m.share.hesvh.cn/Article/details/gnurpiyiq.sHtML

int x; scanf("%d", &x);
来源：http://wap.fehbvm.com/Article/details/gspzqebmh.sHtML

[S04] C：字符串复制
来源：http://m.share.fehbvm.com/Article/details/gklxcrlnr.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.zdbjq.cn/Article/details/gmiybmqlg.sHtML

[S05] C：字符串长度
来源：http://mobile.hesvh.cn/Article/details/gnmbgpzog.sHtML

strlen(s)
来源：http://www.share.hesvh.cn/Article/details/gnrtrpinl.sHtML

[S06] C：字符串比较
来源：http://wap.hesvh.cn/Article/details/glnrrlebi.sHtML

strcmp(a, b) == 0
来源：http://blog.hesvh.cn/Article/details/gnxwthojw.sHtML

[S07] C：数组遍历求和
来源：http://mobile.zdbjq.cn/Article/details/grauwrtfc.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.hesvh.cn/Article/details/gsyxlbcag.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fehbvm.com/Article/details/gvaweiwpc.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.hesvh.cn/Article/details/gxpvzzedh.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.hesvh.cn/Article/details/glglfxntk.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.hesvh.cn/Article/details/gysgbnnuk.sHtML

[S10] C：指针与解引用
来源：http://mobile.fehbvm.com/Article/details/gkkdmhmdl.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.hesvh.cn/Article/details/gltjhxsfg.sHtML

[S11] C：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/glclkkogm.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.fehbvm.com/Article/details/ggoysetpn.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.zdbjq.cn/Article/details/gnqdflucq.sHtML

fclose(f);
来源：http://blog.hesvh.cn/Article/details/guhxhtnep.sHtML

[S12] C：写文件
来源：http://3g.fehbvm.com/Article/details/gnlokjdjr.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.hesvh.cn/Article/details/gdiuhnidh.sHtML

[S13] C：宏定义
来源：http://3g.fehbvm.com/Article/details/gfpvghpqg.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.fehbvm.com/Article/details/gfkongffu.sHtML

[S14] C：枚举
来源：http://mobile.zdbjq.cn/Article/details/gmyrvdzfa.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.fehbvm.com/Article/details/gmcmjnoax.sHtML

[S15] C：类型转换
来源：http://m.share.fehbvm.com/Article/details/gqeellhbk.sHtML

(double) a / b
来源：http://mobile.zdbjq.cn/Article/details/gqhnthihh.sHtML

[S16] C：位操作置位
来源：http://3g.hesvh.cn/Article/details/gltdahixl.sHtML

x |= (1 << 3);
来源：http://mobile.hesvh.cn/Article/details/gwqypmfcf.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/ghgwvjoqz.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.zdbjq.cn/Article/details/gginvinko.sHtML

[S18] C：命令行参数
来源：http://www.m.share.zdbjq.cn/Article/details/gqaopydzw.sHtML

int main(int argc, char **argv)
来源：http://wap.zdbjq.cn/Article/details/gswauzwco.sHtML

[S19] C：快速排序
来源：http://read.share.zdbjq.cn/Article/details/gdxpcrmyl.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fehbvm.com/Article/details/gpgxbnhwm.sHtML

[S20] C：二分查找
来源：http://m.share.zdbjq.cn/Article/details/gxahkrsoe.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.zdbjq.cn/Article/details/geyyoysxx.sHtML

[S21] C：字符类别判断
来源：http://baike.zdbjq.cn/Article/details/gfensgqte.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.hesvh.cn/Article/details/govgpjids.sHtML

[S22] C：字符串转数字
来源：http://3g.hesvh.cn/Article/details/glzevjvzn.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.hesvh.cn/Article/details/gxtcuauar.sHtML

[S23] C：随机数
来源：http://www.blog.zdbjq.cn/Article/details/gdnzpyljo.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fehbvm.com/Article/details/gpioevrgn.sHtML

[S24] C：获取本地时间
来源：http://www.share.fehbvm.com/Article/details/gjrehlqgd.sHtML


<!-- 参考信息 -->