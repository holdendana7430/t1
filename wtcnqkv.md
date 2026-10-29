代发 wailian999

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.zdbjq.cn/Article/details/gqqzttalr.sHtML

[Q52] 删除指定行
来源：http://blog.fehbvm.com/Article/details/ginomslae.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.fehbvm.com/Article/details/gspxolids.sHtML

[Q53] 按条件删除
来源：http://blog.hesvh.cn/Article/details/glrelbriw.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.zdbjq.cn/Article/details/gxclqzivj.sHtML

[Q54] 清空表
来源：http://www.blog.hesvh.cn/Article/details/gmmoyuvzl.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.zdbjq.cn/Article/details/ghtdfofhr.sHtML

[Q55] 排名（并列占位）
来源：http://wap.zdbjq.cn/Article/details/goczlqcqa.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.zdbjq.cn/Article/details/gpiybirup.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.zdbjq.cn/Article/details/gbvjuhztv.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.hesvh.cn/Article/details/gdvbozjoz.sHtML

[Q57] 行号
来源：http://read.share.hesvh.cn/Article/details/guaatvtzm.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.hesvh.cn/Article/details/gfrjdcpee.sHtML

[Q58] 累计求和
来源：http://www.share.zdbjq.cn/Article/details/gkbajmtrj.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gqipfryua.sHtML

[Q59] 分组内累计
来源：http://www.m.share.zdbjq.cn/Article/details/gsdlzpwif.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.fehbvm.com/Article/details/glareydal.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.fehbvm.com/Article/details/gxbqpmoic.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.zdbjq.cn/Article/details/gbrnbuvjp.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.fehbvm.com/Article/details/ggljjdqzg.sHtML

[Q61] 移动平均
来源：http://www.m.share.hesvh.cn/Article/details/gggxybhri.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.fehbvm.com/Article/details/gkbnygqqu.sHtML

[Q62] 分组占比
来源：http://3g.fehbvm.com/Article/details/gdtfvpvvs.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/gosgxselx.sHtML

[Q63] 开启事务
来源：http://3g.hesvh.cn/Article/details/gozwywlup.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.zdbjq.cn/Article/details/gbdvwideb.sHtML

[Q64] 提交事务
来源：http://www.m.share.zdbjq.cn/Article/details/gnkiipcmo.sHtML

COMMIT;
来源：http://m.share.hesvh.cn/Article/details/gmpmjhcap.sHtML

[Q65] 回滚事务
来源：http://read.share.hesvh.cn/Article/details/gdcsrenpa.sHtML

ROLLBACK;
来源：http://www.blog.fehbvm.com/Article/details/gwibuyczl.sHtML

[Q66] 行锁查询
来源：http://wap.fehbvm.com/Article/details/gouduqtuq.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.fehbvm.com/Article/details/glhnrlxzz.sHtML

[Q67] 设置隔离级别
来源：http://mobile.hesvh.cn/Article/details/gttfvfsoi.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.fehbvm.com/Article/details/gzhnaobrv.sHtML

[Q68] 保存点
来源：http://www.blog.zdbjq.cn/Article/details/gkmmsgnfp.sHtML

SAVEPOINT sp1;
来源：http://www.blog.fehbvm.com/Article/details/guspyyltg.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.fehbvm.com/Article/details/gqslflfsp.sHtML

[Q69] 查看执行计划
来源：http://www.blog.zdbjq.cn/Article/details/gzcvcoyoc.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.fehbvm.com/Article/details/gvpfmxbxb.sHtML

[Q70] 更新统计信息
来源：http://www.blog.fehbvm.com/Article/details/gidduggrm.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.fehbvm.com/Article/details/grkgnwsbx.sHtML

[Q71] 查看建表语句
来源：http://mobile.fehbvm.com/Article/details/gvrgcivwn.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.hesvh.cn/Article/details/gpyuixuvr.sHtML

[Q72] 查看索引
来源：http://www.m.share.zdbjq.cn/Article/details/gscpofxgr.sHtML

SHOW INDEX FROM users;
来源：http://blog.fehbvm.com/Article/details/gkvrhkcnv.sHtML

[Q73] 查看表状态
来源：http://www.blog.hesvh.cn/Article/details/gstomcbzy.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.hesvh.cn/Article/details/gotybebul.sHtML

[Q74] 强制使用索引
来源：http://www.share.zdbjq.cn/Article/details/gmflubfls.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.hesvh.cn/Article/details/gkgzkrhkl.sHtML

[Q75] 日期格式化
来源：http://baike.fehbvm.com/Article/details/gclrgtdbg.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.zdbjq.cn/Article/details/glspxbdui.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.hesvh.cn/Article/details/gpqattxeq.sHtML

[Q76] 按天统计
来源：http://www.m.share.zdbjq.cn/Article/details/gdydunoqf.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.fehbvm.com/Article/details/gdmdwthcd.sHtML

[Q77] 时间加减
来源：http://baike.fehbvm.com/Article/details/gontkallp.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.fehbvm.com/Article/details/gkrgbwmwv.sHtML

[Q78] 当前时间
来源：http://m.share.zdbjq.cn/Article/details/ggrvnhvlz.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.zdbjq.cn/Article/details/gidavsxrb.sHtML

[Q79] 字符串拼接
来源：http://m.share.zdbjq.cn/Article/details/gjyijkhwt.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.zdbjq.cn/Article/details/grrrlfgny.sHtML

[Q80] 字符串截取
来源：http://blog.zdbjq.cn/Article/details/ggfownhuo.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.fehbvm.com/Article/details/ggklxxsqs.sHtML

[Q81] 字符串替换
来源：http://read.share.zdbjq.cn/Article/details/gkrxolojf.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.fehbvm.com/Article/details/gemtwaxtt.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.fehbvm.com/Article/details/gravcqjba.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gxkyylzdd.sHtML

[Q83] 大小写转换
来源：http://www.share.zdbjq.cn/Article/details/ghbiixipn.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/glmpsnqjj.sHtML

[Q84] 去除首尾空格
来源：http://www.share.zdbjq.cn/Article/details/gfexwbxpt.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gkkcevbcd.sHtML

[Q85] 数值取整
来源：http://baike.zdbjq.cn/Article/details/gcwfgzmjd.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.hesvh.cn/Article/details/gerjlerhk.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.fehbvm.com/Article/details/gdgepfkde.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.hesvh.cn/Article/details/gvzeaeuxa.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.hesvh.cn/Article/details/gemapyfmx.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.fehbvm.com/Article/details/ggisaxjte.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.zdbjq.cn/Article/details/gyvgqvgmy.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.fehbvm.com/Article/details/gvxlfewkw.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gvrbdpsxb.sHtML

[Q89] 判断表是否存在
来源：http://www.share.zdbjq.cn/Article/details/glrzbivkf.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.zdbjq.cn/Article/details/gtpvoojwn.sHtML

[Q90] 生成序号列
来源：http://www.share.zdbjq.cn/Article/details/gqrgsvyzc.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.hesvh.cn/Article/details/gblysebnc.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gzerbktvx.sHtML

R. Bash 专题
来源：http://read.share.hesvh.cn/Article/details/gexnrnsth.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gfkyrhhhk.sHtML

[R01] shebang 与严格模式
来源：http://www.share.fehbvm.com/Article/details/gecwkbjbc.sHtML

#!/usr/bin/env bash
来源：http://www.share.hesvh.cn/Article/details/gnqaahbzx.sHtML

set -euo pipefail
来源：http://m.share.fehbvm.com/Article/details/gctjmdomr.sHtML

[R02] 变量赋值与使用
来源：http://baike.zdbjq.cn/Article/details/govyzusgm.sHtML

name="Tom"; echo "$name"
来源：http://m.share.zdbjq.cn/Article/details/gcvboiehg.sHtML

[R03] 只读变量
来源：http://3g.fehbvm.com/Article/details/gatramcqs.sHtML

readonly PI=3.14
来源：http://www.m.share.zdbjq.cn/Article/details/goonikfja.sHtML

[R04] 位置参数
来源：http://wap.zdbjq.cn/Article/details/gwrmmyhlz.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.fehbvm.com/Article/details/gzoyaksed.sHtML

[R05] 参数默认值
来源：http://baike.hesvh.cn/Article/details/gzdvrnjdf.sHtML

name="${1:-default}"
来源：http://www.blog.fehbvm.com/Article/details/gcdsphyzv.sHtML

[R06] 判断命令是否存在
来源：http://blog.hesvh.cn/Article/details/gpllcqrrj.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.fehbvm.com/Article/details/gttvujkjp.sHtML

[R07] if 判断文件
来源：http://blog.zdbjq.cn/Article/details/gdqxejvjk.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.fehbvm.com/Article/details/gxyiblzdr.sHtML

[R08] 数值比较
来源：http://www.m.share.hesvh.cn/Article/details/ghxgchyuh.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.fehbvm.com/Article/details/gqvxfyyzb.sHtML

[R09] 字符串比较
来源：http://blog.hesvh.cn/Article/details/gpnsgcxrn.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.fehbvm.com/Article/details/grumqehlq.sHtML

[R10] 正则匹配
来源：http://www.share.fehbvm.com/Article/details/gfdxxzyjr.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.zdbjq.cn/Article/details/ghndzacbd.sHtML

[R11] case 多分支
来源：http://baike.fehbvm.com/Article/details/govgnmoze.sHtML

case "$1" in
来源：http://www.blog.hesvh.cn/Article/details/gzkhylggc.sHtML

start) echo "启动" ;;
来源：http://blog.fehbvm.com/Article/details/gxgiovbil.sHtML

stop)  echo "停止" ;;
来源：http://3g.zdbjq.cn/Article/details/gatchidgc.sHtML

*)     echo "未知命令" ;;
来源：http://baike.zdbjq.cn/Article/details/guerrrnqv.sHtML

esac
来源：http://mobile.fehbvm.com/Article/details/gfupuvmkx.sHtML

[R12] for 遍历文件
来源：http://blog.fehbvm.com/Article/details/gdjnaokpj.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.fehbvm.com/Article/details/gipfusafx.sHtML

[R13] for 计数循环
来源：http://3g.zdbjq.cn/Article/details/gdbnrzdcp.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.hesvh.cn/Article/details/gixxifrfx.sHtML

[R14] C 风格 for
来源：http://baike.hesvh.cn/Article/details/gdtqmjgcs.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.fehbvm.com/Article/details/gxfsagoav.sHtML

[R15] while 逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gmphsrkaq.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.fehbvm.com/Article/details/gatewusvq.sHtML

[R16] until 等待条件
来源：http://www.blog.hesvh.cn/Article/details/gqklwjkew.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.hesvh.cn/Article/details/gxkdnqjes.sHtML

[R17] 数组定义与取值
来源：http://baike.fehbvm.com/Article/details/glnsxpvua.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fehbvm.com/Article/details/grunrvxol.sHtML

[R18] 遍历数组
来源：http://blog.zdbjq.cn/Article/details/glywygzki.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.zdbjq.cn/Article/details/gychoukjo.sHtML

[R19] 数组长度
来源：http://baike.zdbjq.cn/Article/details/gubrmidch.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.hesvh.cn/Article/details/gdatijdae.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.hesvh.cn/Article/details/gdpaduqny.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.fehbvm.com/Article/details/gygbybjfs.sHtML

[R21] 字符串长度
来源：http://mobile.fehbvm.com/Article/details/gfpjyjgip.sHtML

echo "${#s}"
来源：http://m.share.zdbjq.cn/Article/details/gzuiumbbi.sHtML

[R22] 截取子串
来源：http://mobile.hesvh.cn/Article/details/gtfzdzvou.sHtML

echo "${s:0:5}"
来源：http://baike.zdbjq.cn/Article/details/gncyokcbk.sHtML

[R23] 字符串替换
来源：http://www.share.hesvh.cn/Article/details/gaxiqxxph.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.fehbvm.com/Article/details/gesroefpi.sHtML

[R24] 大小写转换
来源：http://m.share.zdbjq.cn/Article/details/ghbhmnoho.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.fehbvm.com/Article/details/gmnditvxe.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.hesvh.cn/Article/details/gazbdftwp.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.zdbjq.cn/Article/details/gfklanywz.sHtML

[R26] 命令替换
来源：http://mobile.fehbvm.com/Article/details/gzbbgrpwz.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.fehbvm.com/Article/details/gamssjlja.sHtML

[R27] 算术展开
来源：http://www.blog.hesvh.cn/Article/details/gwnhysbbc.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.fehbvm.com/Article/details/giprtqupc.sHtML

[R28] 浮点运算
来源：http://www.m.share.hesvh.cn/Article/details/grmbicwbi.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.zdbjq.cn/Article/details/gjbindbcr.sHtML

[R29] 定义函数
来源：http://read.share.fehbvm.com/Article/details/gkxfjomla.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.hesvh.cn/Article/details/gpalgckhn.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.hesvh.cn/Article/details/gxxlqzayp.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.fehbvm.com/Article/details/grwpjebtp.sHtML

[R31] 局部变量
来源：http://3g.fehbvm.com/Article/details/gtbmfibzf.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.zdbjq.cn/Article/details/gbnftttsg.sHtML

[R32] 参数个数校验
来源：http://3g.hesvh.cn/Article/details/gkzawbxni.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.hesvh.cn/Article/details/gnxobjpbm.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.hesvh.cn/Article/details/gdgjlupsq.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.fehbvm.com/Article/details/gedvmrndz.sHtML

[R34] 退出时清理
来源：http://m.share.zdbjq.cn/Article/details/gpzmklmvq.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.hesvh.cn/Article/details/glwnxmlxf.sHtML

[R35] 后台执行并等待
来源：http://read.share.zdbjq.cn/Article/details/gauvqsfnn.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.hesvh.cn/Article/details/ghrrhpzwb.sHtML

[R36] 并发执行多个任务
来源：http://wap.zdbjq.cn/Article/details/gyrnooven.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.zdbjq.cn/Article/details/gskmtkyyt.sHtML

[R37] 把输出赋给变量
来源：http://3g.fehbvm.com/Article/details/gtjvbyhfh.sHtML

files=$(ls -1)
来源：http://m.share.hesvh.cn/Article/details/gjaxjhhnv.sHtML

[R38] 管道串联
来源：http://baike.fehbvm.com/Article/details/gmbuwpbse.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.fehbvm.com/Article/details/gcchchedf.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fehbvm.com/Article/details/gmkgsuryg.sHtML

cmd > out.log 2>&1
来源：http://mobile.fehbvm.com/Article/details/gtfgbbdwt.sHtML

[R40] 追加写日志
来源：http://www.share.fehbvm.com/Article/details/gonesxtrx.sHtML

echo "log" >> out.log
来源：http://blog.fehbvm.com/Article/details/gybwdfkfh.sHtML

[R41] 丢弃输出
来源：http://baike.fehbvm.com/Article/details/gqizlgyvh.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.hesvh.cn/Article/details/gyfhoovxw.sHtML

[R42] 输入重定向
来源：http://mobile.zdbjq.cn/Article/details/gxcbsqrir.sHtML

wc -l < a.txt
来源：http://www.blog.hesvh.cn/Article/details/gszunwgzu.sHtML

[R43] 按名字查找文件
来源：http://read.share.fehbvm.com/Article/details/gpskplybd.sHtML

find . -name "*.log" -type f
来源：http://read.share.hesvh.cn/Article/details/gpggimsiu.sHtML

[R44] 按修改时间查找
来源：http://wap.fehbvm.com/Article/details/gbimpehif.sHtML

find . -mtime -7 -type f
来源：http://read.share.hesvh.cn/Article/details/gjreugomy.sHtML

[R45] 批量删除
来源：http://3g.fehbvm.com/Article/details/gqejyofgg.sHtML

find . -name "*.tmp" -delete
来源：http://3g.fehbvm.com/Article/details/ghnksuzrf.sHtML

[R46] 递归替换文件内容
来源：http://wap.zdbjq.cn/Article/details/gjqsawdns.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.hesvh.cn/Article/details/gsqnihmng.sHtML

[R47] sed 单行替换
来源：http://blog.zdbjq.cn/Article/details/gspjavcyq.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.zdbjq.cn/Article/details/gaqmsunlu.sHtML

[R48] awk 取指定列
来源：http://baike.hesvh.cn/Article/details/gampbfqij.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.hesvh.cn/Article/details/gtfvcxfsv.sHtML

[R49] awk 带条件
来源：http://www.blog.fehbvm.com/Article/details/gsosezexg.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fehbvm.com/Article/details/gbxipdnbt.sHtML

[R50] awk 求和
来源：http://blog.hesvh.cn/Article/details/gvmnyrvkq.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.zdbjq.cn/Article/details/gvtipalqv.sHtML

[R51] 排序去重取前几
来源：http://www.blog.zdbjq.cn/Article/details/gdfniorey.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.hesvh.cn/Article/details/guuxxokma.sHtML

[R52] 统计行数
来源：http://read.share.hesvh.cn/Article/details/gojuwjcgb.sHtML

wc -l a.txt
来源：http://wap.zdbjq.cn/Article/details/gevoljlom.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.zdbjq.cn/Article/details/gtazkogyt.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.zdbjq.cn/Article/details/gliozkylp.sHtML

[R54] 比较两个文件
来源：http://www.m.share.zdbjq.cn/Article/details/ghtkudqem.sHtML

diff a.txt b.txt
来源：http://www.share.fehbvm.com/Article/details/gntylwocv.sHtML

[R55] 压缩与解压
来源：http://www.blog.zdbjq.cn/Article/details/gvayupulj.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.hesvh.cn/Article/details/gduhicugx.sHtML

[R56] 远程拷贝
来源：http://baike.fehbvm.com/Article/details/gqmegevli.sHtML

scp file user@host:/path/
来源：http://www.blog.fehbvm.com/Article/details/gfvngrija.sHtML

[R57] 远程执行命令
来源：http://mobile.fehbvm.com/Article/details/glullircn.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.zdbjq.cn/Article/details/gdlatguct.sHtML

[R58] 下载文件
来源：http://mobile.hesvh.cn/Article/details/gnjiikwro.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.zdbjq.cn/Article/details/gjwvjtdml.sHtML

[R59] 发 POST JSON
来源：http://m.share.hesvh.cn/Article/details/gdqdrxgxc.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fehbvm.com/Article/details/gjnrbderx.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.hesvh.cn/Article/details/gffjfmltn.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.hesvh.cn/Article/details/gnzktbfqv.sHtML

[R61] 磁盘占用
来源：http://read.share.hesvh.cn/Article/details/gddxyqcvz.sHtML

df -h;  du -sh *
来源：http://read.share.fehbvm.com/Article/details/giqdthtrz.sHtML

[R62] 找最占空间的文件
来源：http://read.share.hesvh.cn/Article/details/gqnkafcjm.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.fehbvm.com/Article/details/gmffxwahu.sHtML

[R63] 内存与进程
来源：http://www.share.hesvh.cn/Article/details/ghvendvby.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.fehbvm.com/Article/details/gtwqzwszx.sHtML

[R64] 结束进程
来源：http://www.share.hesvh.cn/Article/details/ghdrqgwth.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.hesvh.cn/Article/details/ggfelefhq.sHtML

[R65] 查看端口占用
来源：http://www.share.zdbjq.cn/Article/details/guhzcadmk.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.zdbjq.cn/Article/details/gvwartvbo.sHtML

[R66] 定时任务
来源：http://blog.fehbvm.com/Article/details/gxlgghhjs.sHtML

crontab -e;  crontab -l
来源：http://wap.fehbvm.com/Article/details/gwfvdnipq.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fehbvm.com/Article/details/gkoitcskz.sHtML

openssl rand -hex 16
来源：http://read.share.zdbjq.cn/Article/details/gikqqmvkj.sHtML

[R68] 计算文件校验值
来源：http://m.share.fehbvm.com/Article/details/gronnmmlv.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.zdbjq.cn/Article/details/gakpcmulr.sHtML

[R69] 生成随机密码
来源：http://3g.hesvh.cn/Article/details/guiabzgwc.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.fehbvm.com/Article/details/glbfuarks.sHtML

[R70] 时间戳与互转
来源：http://www.blog.zdbjq.cn/Article/details/ghthuhcfj.sHtML

date +%s;  date -d @1700000000
来源：http://3g.hesvh.cn/Article/details/giqlzukvi.sHtML

[R71] 日期格式化
来源：http://read.share.zdbjq.cn/Article/details/gjthtiuyr.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.fehbvm.com/Article/details/gnmwjwtsu.sHtML

[R72] 等待端口就绪
来源：http://www.share.fehbvm.com/Article/details/gkgmmdila.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fehbvm.com/Article/details/gloktojbf.sHtML

[R73] 分割大日志
来源：http://3g.fehbvm.com/Article/details/gvzfxrqpv.sHtML

split -l 1000 big.log part_
来源：http://baike.zdbjq.cn/Article/details/gvgybuofw.sHtML

[R74] 批量重命名
来源：http://www.m.share.zdbjq.cn/Article/details/goykiieer.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.hesvh.cn/Article/details/gvtuaystr.sHtML

[R75] 导出环境变量
来源：http://wap.hesvh.cn/Article/details/gdxwditpj.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.zdbjq.cn/Article/details/gvzvzqwns.sHtML

[R76] 使用临时文件
来源：http://wap.zdbjq.cn/Article/details/gytpvdest.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fehbvm.com/Article/details/gxerepmbo.sHtML

[R77] 读取用户输入
来源：http://mobile.fehbvm.com/Article/details/gozhzuwrb.sHtML

read -rp "请输入: " ans
来源：http://www.share.hesvh.cn/Article/details/gbjyejvvu.sHtML

[R78] 交互式菜单
来源：http://mobile.hesvh.cn/Article/details/glxaqdyfj.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.hesvh.cn/Article/details/gnwzhlcao.sHtML

[R79] 解析命令行选项
来源：http://baike.zdbjq.cn/Article/details/gwezaeoyh.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.fehbvm.com/Article/details/gbhvziaid.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.fehbvm.com/Article/details/gxfocqyms.sHtML

time ./run.sh
来源：http://read.share.fehbvm.com/Article/details/gaowtfcaw.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gfufkjsms.sHtML

S. C / C++ 专题
来源：http://www.m.share.zdbjq.cn/Article/details/groplfehb.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/grbdddwbi.sHtML

[S01] C：Hello World
来源：http://read.share.fehbvm.com/Article/details/gwkiqjrqq.sHtML

#include <stdio.h>
来源：http://m.share.hesvh.cn/Article/details/gthllwill.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.zdbjq.cn/Article/details/ggwonbaiz.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.hesvh.cn/Article/details/gqyyusskp.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.zdbjq.cn/Article/details/guwyiscil.sHtML

[S03] C：读入整数
来源：http://www.m.share.zdbjq.cn/Article/details/gowmdtfgp.sHtML

int x; scanf("%d", &x);
来源：http://3g.fehbvm.com/Article/details/gpvlfpdqx.sHtML

[S04] C：字符串复制
来源：http://www.blog.fehbvm.com/Article/details/gtqomkvql.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.fehbvm.com/Article/details/gpadcezrl.sHtML

[S05] C：字符串长度
来源：http://3g.fehbvm.com/Article/details/gzrgdgiot.sHtML

strlen(s)
来源：http://mobile.hesvh.cn/Article/details/gjghtxpsz.sHtML

[S06] C：字符串比较
来源：http://blog.fehbvm.com/Article/details/gaqljypfc.sHtML

strcmp(a, b) == 0
来源：http://3g.fehbvm.com/Article/details/gzdgninhq.sHtML

[S07] C：数组遍历求和
来源：http://wap.zdbjq.cn/Article/details/gpvlyflhg.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.zdbjq.cn/Article/details/gwhjtcuzt.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.fehbvm.com/Article/details/gakonwdtu.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fehbvm.com/Article/details/gsuuslipk.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.hesvh.cn/Article/details/gjarfefta.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.hesvh.cn/Article/details/ghhvzlwjy.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.hesvh.cn/Article/details/gywviwbhm.sHtML

int *p = &a;  *p = 5;
来源：http://wap.hesvh.cn/Article/details/gpigjnnfs.sHtML

[S11] C：逐行读文件
来源：http://blog.zdbjq.cn/Article/details/grryxllkm.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.zdbjq.cn/Article/details/gbwyczlli.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.fehbvm.com/Article/details/gvfyuzdfp.sHtML

fclose(f);
来源：http://read.share.fehbvm.com/Article/details/gtbxsijgs.sHtML

[S12] C：写文件
来源：http://www.share.hesvh.cn/Article/details/gbookdmem.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.fehbvm.com/Article/details/ghgkugdei.sHtML

[S13] C：宏定义
来源：http://blog.hesvh.cn/Article/details/gffconryl.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.zdbjq.cn/Article/details/gaawiqeui.sHtML

[S14] C：枚举
来源：http://baike.fehbvm.com/Article/details/ggscvlaxi.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.zdbjq.cn/Article/details/gyexuplwl.sHtML

[S15] C：类型转换
来源：http://www.blog.hesvh.cn/Article/details/gmvzlvuvr.sHtML

(double) a / b
来源：http://baike.zdbjq.cn/Article/details/gqjolhtfp.sHtML

[S16] C：位操作置位
来源：http://wap.zdbjq.cn/Article/details/geakomnrv.sHtML

x |= (1 << 3);
来源：http://www.share.hesvh.cn/Article/details/guykxlutd.sHtML

[S17] C：安全拼接字符串
来源：http://baike.fehbvm.com/Article/details/gjmkhurmv.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fehbvm.com/Article/details/gttdcjucn.sHtML

[S18] C：命令行参数
来源：http://www.share.hesvh.cn/Article/details/gswctcpna.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.hesvh.cn/Article/details/glppopgil.sHtML

[S19] C：快速排序
来源：http://read.share.zdbjq.cn/Article/details/gzpcjzjam.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fehbvm.com/Article/details/gjzwsjyul.sHtML

[S20] C：二分查找
来源：http://www.blog.fehbvm.com/Article/details/gvshkgyco.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.fehbvm.com/Article/details/goajrgjch.sHtML

[S21] C：字符类别判断
来源：http://wap.hesvh.cn/Article/details/gksqnpdvx.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.fehbvm.com/Article/details/gwmmssqkh.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fehbvm.com/Article/details/gdhwvtoql.sHtML


<!-- 参考信息 -->