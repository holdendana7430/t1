代发 wailian999

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.hesvh.cn/Article/details/gpetqwnkz.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.hesvh.cn/Article/details/gtuieomwm.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.zdbjq.cn/Article/details/gxfakyzis.sHtML

[Q57] 行号
来源：http://read.share.zdbjq.cn/Article/details/gywaqrmjy.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.zdbjq.cn/Article/details/gwlwyzyem.sHtML

[Q58] 累计求和
来源：http://www.blog.hesvh.cn/Article/details/gdaotigmv.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.hesvh.cn/Article/details/gbhzhwjtr.sHtML

[Q59] 分组内累计
来源：http://3g.zdbjq.cn/Article/details/gcmijzbsq.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gveosqzog.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.fehbvm.com/Article/details/gmclbolko.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.hesvh.cn/Article/details/gwlnyavmg.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/ggebzbdal.sHtML

[Q61] 移动平均
来源：http://blog.zdbjq.cn/Article/details/goowlipxc.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gerpemysp.sHtML

[Q62] 分组占比
来源：http://baike.hesvh.cn/Article/details/gkidjopho.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.hesvh.cn/Article/details/gcwfwmyox.sHtML

[Q63] 开启事务
来源：http://www.share.zdbjq.cn/Article/details/gvonfbcib.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.fehbvm.com/Article/details/givvqaqwu.sHtML

[Q64] 提交事务
来源：http://www.share.fehbvm.com/Article/details/geyyzbrmv.sHtML

COMMIT;
来源：http://3g.hesvh.cn/Article/details/gcpilugpu.sHtML

[Q65] 回滚事务
来源：http://wap.zdbjq.cn/Article/details/gvfarhfdt.sHtML

ROLLBACK;
来源：http://www.m.share.zdbjq.cn/Article/details/gcdatovbi.sHtML

[Q66] 行锁查询
来源：http://wap.zdbjq.cn/Article/details/gtijdedua.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.zdbjq.cn/Article/details/gjaxilywj.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.fehbvm.com/Article/details/gxhnwdtry.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.fehbvm.com/Article/details/gkxcqnrmx.sHtML

[Q68] 保存点
来源：http://3g.fehbvm.com/Article/details/gjfegopda.sHtML

SAVEPOINT sp1;
来源：http://3g.fehbvm.com/Article/details/gcqkukwjy.sHtML

ROLLBACK TO sp1;
来源：http://m.share.fehbvm.com/Article/details/gjfpcsbxt.sHtML

[Q69] 查看执行计划
来源：http://baike.hesvh.cn/Article/details/gemexlpje.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.fehbvm.com/Article/details/gqfnpyvoi.sHtML

[Q70] 更新统计信息
来源：http://blog.zdbjq.cn/Article/details/gizdruily.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.hesvh.cn/Article/details/gwigkgmyj.sHtML

[Q71] 查看建表语句
来源：http://www.blog.zdbjq.cn/Article/details/givqiivtk.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.hesvh.cn/Article/details/gbzawovvs.sHtML

[Q72] 查看索引
来源：http://3g.fehbvm.com/Article/details/gydpoptjl.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gnszkkamz.sHtML

[Q73] 查看表状态
来源：http://blog.hesvh.cn/Article/details/guowdpibj.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.fehbvm.com/Article/details/gakzpchdr.sHtML

[Q74] 强制使用索引
来源：http://blog.hesvh.cn/Article/details/gtsawlbag.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.hesvh.cn/Article/details/gauhmraog.sHtML

[Q75] 日期格式化
来源：http://3g.fehbvm.com/Article/details/gmfvjmnup.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gitrjgsyq.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.zdbjq.cn/Article/details/ggbffnxaa.sHtML

[Q76] 按天统计
来源：http://m.share.fehbvm.com/Article/details/gfncrpclm.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.fehbvm.com/Article/details/gxxxnxtia.sHtML

[Q77] 时间加减
来源：http://m.share.hesvh.cn/Article/details/gveunkzjf.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.fehbvm.com/Article/details/gtoxvjgxh.sHtML

[Q78] 当前时间
来源：http://mobile.hesvh.cn/Article/details/gdoqvcqru.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.hesvh.cn/Article/details/gjwuwjnfa.sHtML

[Q79] 字符串拼接
来源：http://blog.zdbjq.cn/Article/details/gmfcohkhx.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.hesvh.cn/Article/details/gxwkuawwn.sHtML

[Q80] 字符串截取
来源：http://m.share.hesvh.cn/Article/details/gdgtyhycn.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gvphqvseu.sHtML

[Q81] 字符串替换
来源：http://3g.zdbjq.cn/Article/details/gtnddwzef.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.hesvh.cn/Article/details/gjaqnggat.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.fehbvm.com/Article/details/gagynwear.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gtatxtmxj.sHtML

[Q83] 大小写转换
来源：http://www.m.share.hesvh.cn/Article/details/gjmwfmvrk.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gezhunkrh.sHtML

[Q84] 去除首尾空格
来源：http://m.share.zdbjq.cn/Article/details/gfaaqakwc.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gykgshvak.sHtML

[Q85] 数值取整
来源：http://read.share.hesvh.cn/Article/details/gzbkaqkmm.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.hesvh.cn/Article/details/gzmwslqxr.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.zdbjq.cn/Article/details/grnbabbaj.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.zdbjq.cn/Article/details/ghmixsszw.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.fehbvm.com/Article/details/gvazjcttv.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.fehbvm.com/Article/details/gbnhhxgsp.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.hesvh.cn/Article/details/giwsmmaft.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.fehbvm.com/Article/details/gravjtflh.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.hesvh.cn/Article/details/ggkczzsua.sHtML

[Q89] 判断表是否存在
来源：http://blog.fehbvm.com/Article/details/geykwanvf.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.fehbvm.com/Article/details/gourcwxor.sHtML

[Q90] 生成序号列
来源：http://baike.fehbvm.com/Article/details/gzbphpaap.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.fehbvm.com/Article/details/gndtszlol.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gfqqfgkan.sHtML

R. Bash 专题
来源：http://www.blog.hesvh.cn/Article/details/gtzqulbcz.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gquybntft.sHtML

[R01] shebang 与严格模式
来源：http://www.share.fehbvm.com/Article/details/gmpwklweo.sHtML

#!/usr/bin/env bash
来源：http://read.share.fehbvm.com/Article/details/gzirwmvwe.sHtML

set -euo pipefail
来源：http://3g.hesvh.cn/Article/details/grvabvoyj.sHtML

[R02] 变量赋值与使用
来源：http://read.share.hesvh.cn/Article/details/gqpjlbecu.sHtML

name="Tom"; echo "$name"
来源：http://m.share.fehbvm.com/Article/details/gdrxsxgvj.sHtML

[R03] 只读变量
来源：http://baike.fehbvm.com/Article/details/gaivndmnl.sHtML

readonly PI=3.14
来源：http://wap.zdbjq.cn/Article/details/gazqdrdgm.sHtML

[R04] 位置参数
来源：http://blog.hesvh.cn/Article/details/gnbsojolc.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.hesvh.cn/Article/details/gmucarqvt.sHtML

[R05] 参数默认值
来源：http://www.share.fehbvm.com/Article/details/gtuzcptzb.sHtML

name="${1:-default}"
来源：http://www.m.share.hesvh.cn/Article/details/gkuogdfam.sHtML

[R06] 判断命令是否存在
来源：http://blog.zdbjq.cn/Article/details/ggejikmvi.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.zdbjq.cn/Article/details/gxxzgikhf.sHtML

[R07] if 判断文件
来源：http://wap.fehbvm.com/Article/details/gzmevofqf.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gynidknxk.sHtML

[R08] 数值比较
来源：http://blog.fehbvm.com/Article/details/gdtdvpezi.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.hesvh.cn/Article/details/gqjkoqqeb.sHtML

[R09] 字符串比较
来源：http://wap.fehbvm.com/Article/details/gvppiaaos.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.zdbjq.cn/Article/details/gnwrpiyxo.sHtML

[R10] 正则匹配
来源：http://www.blog.fehbvm.com/Article/details/gwpgeaipn.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gwsvmotdz.sHtML

[R11] case 多分支
来源：http://3g.hesvh.cn/Article/details/gdxjssqmu.sHtML

case "$1" in
来源：http://m.share.fehbvm.com/Article/details/gktdujonn.sHtML

start) echo "启动" ;;
来源：http://www.blog.fehbvm.com/Article/details/gbhiutkvq.sHtML

stop)  echo "停止" ;;
来源：http://www.share.zdbjq.cn/Article/details/gutxkezlu.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.fehbvm.com/Article/details/grbppetac.sHtML

esac
来源：http://www.m.share.hesvh.cn/Article/details/goqbxisga.sHtML

[R12] for 遍历文件
来源：http://mobile.fehbvm.com/Article/details/ghznniggo.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.zdbjq.cn/Article/details/gnnzqoqmj.sHtML

[R13] for 计数循环
来源：http://m.share.hesvh.cn/Article/details/gpvjceojw.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.fehbvm.com/Article/details/gobrxixvo.sHtML

[R14] C 风格 for
来源：http://read.share.hesvh.cn/Article/details/ggrhrinez.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.zdbjq.cn/Article/details/ggcgyjkql.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gziardkdc.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.hesvh.cn/Article/details/gmwjvkawq.sHtML

[R16] until 等待条件
来源：http://wap.fehbvm.com/Article/details/gcejsrnem.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.zdbjq.cn/Article/details/gewafhdne.sHtML

[R17] 数组定义与取值
来源：http://mobile.fehbvm.com/Article/details/goasnegcg.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.fehbvm.com/Article/details/gxkrtypil.sHtML

[R18] 遍历数组
来源：http://baike.hesvh.cn/Article/details/gxuoaofwi.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.zdbjq.cn/Article/details/gugcskrkm.sHtML

[R19] 数组长度
来源：http://3g.fehbvm.com/Article/details/gdgkmxwhn.sHtML

echo "${#arr[@]}"
来源：http://3g.zdbjq.cn/Article/details/gafltanjc.sHtML

[R20] 关联数组（字典）
来源：http://wap.zdbjq.cn/Article/details/ggeoxbqkr.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.fehbvm.com/Article/details/gxjcpmqgj.sHtML

[R21] 字符串长度
来源：http://read.share.zdbjq.cn/Article/details/gcmxnhqme.sHtML

echo "${#s}"
来源：http://wap.hesvh.cn/Article/details/gpnfcnxbe.sHtML

[R22] 截取子串
来源：http://blog.zdbjq.cn/Article/details/gsersslfy.sHtML

echo "${s:0:5}"
来源：http://www.m.share.fehbvm.com/Article/details/glkvundrt.sHtML

[R23] 字符串替换
来源：http://www.blog.fehbvm.com/Article/details/gocscurno.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fehbvm.com/Article/details/giaqyuinf.sHtML

[R24] 大小写转换
来源：http://www.m.share.zdbjq.cn/Article/details/gvplrchwi.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fehbvm.com/Article/details/gwdtqylbz.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.zdbjq.cn/Article/details/gtbwcsbwp.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.hesvh.cn/Article/details/gzxqmktcz.sHtML

[R26] 命令替换
来源：http://www.share.hesvh.cn/Article/details/gwknqvjaf.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.fehbvm.com/Article/details/gphmvdter.sHtML

[R27] 算术展开
来源：http://m.share.zdbjq.cn/Article/details/goxvvyyqn.sHtML

echo $((1 + 2 * 3))
来源：http://baike.hesvh.cn/Article/details/gxgvqjifx.sHtML

[R28] 浮点运算
来源：http://www.share.zdbjq.cn/Article/details/gerpteyxh.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.zdbjq.cn/Article/details/gpaejjxbh.sHtML

[R29] 定义函数
来源：http://m.share.zdbjq.cn/Article/details/gqnxtblin.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.fehbvm.com/Article/details/gaklzybgv.sHtML

[R30] 函数返回状态码
来源：http://www.share.fehbvm.com/Article/details/gtpzuzqaq.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.fehbvm.com/Article/details/gpqbweeqs.sHtML

[R31] 局部变量
来源：http://www.blog.zdbjq.cn/Article/details/gbelzdopm.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.zdbjq.cn/Article/details/gynbfpgrt.sHtML

[R32] 参数个数校验
来源：http://www.blog.zdbjq.cn/Article/details/ggzofjerg.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.zdbjq.cn/Article/details/gwmanbwip.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.hesvh.cn/Article/details/gecsskkpv.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.hesvh.cn/Article/details/gwdcxmvrv.sHtML

[R34] 退出时清理
来源：http://www.share.zdbjq.cn/Article/details/geibjzqkx.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.hesvh.cn/Article/details/gxblmmygg.sHtML

[R35] 后台执行并等待
来源：http://baike.zdbjq.cn/Article/details/gsfrkfyxq.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fehbvm.com/Article/details/gqivmycwk.sHtML

[R36] 并发执行多个任务
来源：http://m.share.hesvh.cn/Article/details/ggeqgtujw.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.fehbvm.com/Article/details/gxlctghvp.sHtML

[R37] 把输出赋给变量
来源：http://wap.zdbjq.cn/Article/details/geyfeajbd.sHtML

files=$(ls -1)
来源：http://www.blog.hesvh.cn/Article/details/gdrqkjwpw.sHtML

[R38] 管道串联
来源：http://www.blog.hesvh.cn/Article/details/gpgtdgzjo.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.fehbvm.com/Article/details/gcgjcasau.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.hesvh.cn/Article/details/ggjgexwvk.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.hesvh.cn/Article/details/gyzyxgmkb.sHtML

[R40] 追加写日志
来源：http://blog.hesvh.cn/Article/details/gbtgexlts.sHtML

echo "log" >> out.log
来源：http://read.share.fehbvm.com/Article/details/glrqocubk.sHtML

[R41] 丢弃输出
来源：http://www.m.share.hesvh.cn/Article/details/gutuwnjkm.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fehbvm.com/Article/details/ggxuudlia.sHtML

[R42] 输入重定向
来源：http://www.blog.zdbjq.cn/Article/details/gppxazmkb.sHtML

wc -l < a.txt
来源：http://www.share.hesvh.cn/Article/details/gbtltjjti.sHtML

[R43] 按名字查找文件
来源：http://www.blog.fehbvm.com/Article/details/gqjamszcv.sHtML

find . -name "*.log" -type f
来源：http://baike.zdbjq.cn/Article/details/gojoryoiv.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.zdbjq.cn/Article/details/gibicvuuv.sHtML

find . -mtime -7 -type f
来源：http://m.share.hesvh.cn/Article/details/gmmgdqtgu.sHtML

[R45] 批量删除
来源：http://wap.hesvh.cn/Article/details/gklygfsrc.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.zdbjq.cn/Article/details/gobiphzfw.sHtML

[R46] 递归替换文件内容
来源：http://baike.fehbvm.com/Article/details/gmfdfroyo.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.fehbvm.com/Article/details/gmyrrvogu.sHtML

[R47] sed 单行替换
来源：http://3g.zdbjq.cn/Article/details/grcomehfq.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fehbvm.com/Article/details/gxrxxchjn.sHtML

[R48] awk 取指定列
来源：http://m.share.hesvh.cn/Article/details/gxkwnlmvp.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.zdbjq.cn/Article/details/gsmlcyhyo.sHtML

[R49] awk 带条件
来源：http://wap.hesvh.cn/Article/details/ggcnnalki.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.fehbvm.com/Article/details/gvahlekqb.sHtML

[R50] awk 求和
来源：http://www.share.hesvh.cn/Article/details/gufwkhkvc.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.fehbvm.com/Article/details/grmlnjpha.sHtML

[R51] 排序去重取前几
来源：http://baike.fehbvm.com/Article/details/gepaxdhci.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.hesvh.cn/Article/details/gkzdqhwrj.sHtML

[R52] 统计行数
来源：http://3g.hesvh.cn/Article/details/gewdavhgn.sHtML

wc -l a.txt
来源：http://m.share.fehbvm.com/Article/details/grofhslfv.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.zdbjq.cn/Article/details/gmhwndqaf.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.zdbjq.cn/Article/details/gzstuanll.sHtML

[R54] 比较两个文件
来源：http://baike.hesvh.cn/Article/details/glgqvewqk.sHtML

diff a.txt b.txt
来源：http://www.m.share.hesvh.cn/Article/details/gyhoyjifh.sHtML

[R55] 压缩与解压
来源：http://read.share.fehbvm.com/Article/details/geropfiac.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.zdbjq.cn/Article/details/gccnmqjvs.sHtML

[R56] 远程拷贝
来源：http://m.share.fehbvm.com/Article/details/gklflbzrs.sHtML

scp file user@host:/path/
来源：http://www.share.hesvh.cn/Article/details/gnrjdeoih.sHtML

[R57] 远程执行命令
来源：http://www.share.fehbvm.com/Article/details/gxxlyosui.sHtML

ssh user@host 'uptime'
来源：http://baike.zdbjq.cn/Article/details/gxlwwpiyf.sHtML

[R58] 下载文件
来源：http://www.m.share.fehbvm.com/Article/details/gwdrvrqhc.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.zdbjq.cn/Article/details/grffcrudv.sHtML

[R59] 发 POST JSON
来源：http://www.share.hesvh.cn/Article/details/gwdjqhtqa.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fehbvm.com/Article/details/gyqqrlokk.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.hesvh.cn/Article/details/gpdpeqrik.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.hesvh.cn/Article/details/gsbmqropu.sHtML

[R61] 磁盘占用
来源：http://read.share.zdbjq.cn/Article/details/gvxoimxpn.sHtML

df -h;  du -sh *
来源：http://read.share.hesvh.cn/Article/details/gbvovngat.sHtML

[R62] 找最占空间的文件
来源：http://baike.fehbvm.com/Article/details/gizkvesbj.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.hesvh.cn/Article/details/gpnnynkyz.sHtML

[R63] 内存与进程
来源：http://www.m.share.fehbvm.com/Article/details/gjkfbmezz.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.fehbvm.com/Article/details/gnkjlmozr.sHtML

[R64] 结束进程
来源：http://baike.zdbjq.cn/Article/details/gbprcwsln.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.hesvh.cn/Article/details/gynftxqwb.sHtML

[R65] 查看端口占用
来源：http://m.share.fehbvm.com/Article/details/glruqqnif.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.zdbjq.cn/Article/details/gjfmreaai.sHtML

[R66] 定时任务
来源：http://mobile.fehbvm.com/Article/details/gdssecllm.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.hesvh.cn/Article/details/gqdqeotzu.sHtML

[R67] 生成随机十六进制串
来源：http://blog.zdbjq.cn/Article/details/ggrzgluvc.sHtML

openssl rand -hex 16
来源：http://mobile.zdbjq.cn/Article/details/gbocxdnlq.sHtML

[R68] 计算文件校验值
来源：http://www.share.zdbjq.cn/Article/details/gyawdybvi.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.fehbvm.com/Article/details/grkgzzmyf.sHtML

[R69] 生成随机密码
来源：http://www.share.fehbvm.com/Article/details/geijvpovr.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fehbvm.com/Article/details/gtgeyukam.sHtML

[R70] 时间戳与互转
来源：http://www.share.zdbjq.cn/Article/details/gsmndhmfq.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.zdbjq.cn/Article/details/gbqxvkcao.sHtML

[R71] 日期格式化
来源：http://m.share.hesvh.cn/Article/details/gvadnrass.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.hesvh.cn/Article/details/gfjzluwhm.sHtML

[R72] 等待端口就绪
来源：http://baike.hesvh.cn/Article/details/gjyzhzeri.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fehbvm.com/Article/details/gweirlell.sHtML

[R73] 分割大日志
来源：http://www.m.share.fehbvm.com/Article/details/ghiovhhlu.sHtML

split -l 1000 big.log part_
来源：http://blog.zdbjq.cn/Article/details/gzhlakqsr.sHtML

[R74] 批量重命名
来源：http://baike.hesvh.cn/Article/details/gdnithxji.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.zdbjq.cn/Article/details/gvnzpgaus.sHtML

[R75] 导出环境变量
来源：http://baike.fehbvm.com/Article/details/guzqwrcvb.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.hesvh.cn/Article/details/gwqawygqs.sHtML

[R76] 使用临时文件
来源：http://3g.zdbjq.cn/Article/details/gvdgqujjj.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.zdbjq.cn/Article/details/gvudvgcdn.sHtML

[R77] 读取用户输入
来源：http://blog.hesvh.cn/Article/details/ghkncpmzl.sHtML

read -rp "请输入: " ans
来源：http://3g.hesvh.cn/Article/details/goozwjjhv.sHtML

[R78] 交互式菜单
来源：http://www.blog.fehbvm.com/Article/details/ggljmzcdj.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.zdbjq.cn/Article/details/gedqyzetg.sHtML

[R79] 解析命令行选项
来源：http://blog.hesvh.cn/Article/details/ggkpvxfxx.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.hesvh.cn/Article/details/gkgzcxddh.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.hesvh.cn/Article/details/gnlcxqzrg.sHtML

time ./run.sh
来源：http://3g.zdbjq.cn/Article/details/gkwrxaiqu.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gdqxmdbyr.sHtML

S. C / C++ 专题
来源：http://mobile.zdbjq.cn/Article/details/geptbkgvb.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gnpmspogl.sHtML

[S01] C：Hello World
来源：http://3g.fehbvm.com/Article/details/gtvyaqhsz.sHtML

#include <stdio.h>
来源：http://www.m.share.zdbjq.cn/Article/details/goxpelikv.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.hesvh.cn/Article/details/grsxbowto.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.hesvh.cn/Article/details/ggtfcclva.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.zdbjq.cn/Article/details/giwwrufsu.sHtML

[S03] C：读入整数
来源：http://blog.zdbjq.cn/Article/details/gzeknlbao.sHtML

int x; scanf("%d", &x);
来源：http://baike.hesvh.cn/Article/details/gzxcgttag.sHtML

[S04] C：字符串复制
来源：http://blog.fehbvm.com/Article/details/gnovwaxij.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.fehbvm.com/Article/details/gedfuoegq.sHtML

[S05] C：字符串长度
来源：http://www.m.share.fehbvm.com/Article/details/gxzewztti.sHtML

strlen(s)
来源：http://mobile.hesvh.cn/Article/details/geycbzcdj.sHtML

[S06] C：字符串比较
来源：http://blog.zdbjq.cn/Article/details/ghyywhhka.sHtML

strcmp(a, b) == 0
来源：http://www.share.hesvh.cn/Article/details/geiyfqqme.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fehbvm.com/Article/details/gjwtnulbc.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.zdbjq.cn/Article/details/grbkwifjt.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.zdbjq.cn/Article/details/gpyqibjdf.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.zdbjq.cn/Article/details/gaqbdzrtm.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.hesvh.cn/Article/details/gpqmjpbnz.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.hesvh.cn/Article/details/ggvhwyrul.sHtML

[S10] C：指针与解引用
来源：http://www.blog.hesvh.cn/Article/details/gtpsnjimt.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.hesvh.cn/Article/details/gnbojelkh.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gxlflmvrb.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.fehbvm.com/Article/details/gfseqjlya.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.fehbvm.com/Article/details/gxayyxajr.sHtML

fclose(f);
来源：http://www.share.zdbjq.cn/Article/details/ggexnvlxb.sHtML

[S12] C：写文件
来源：http://baike.zdbjq.cn/Article/details/gapnythya.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.zdbjq.cn/Article/details/gichaivub.sHtML

[S13] C：宏定义
来源：http://m.share.fehbvm.com/Article/details/grhpwuzlz.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.zdbjq.cn/Article/details/gkmlwpotk.sHtML

[S14] C：枚举
来源：http://read.share.fehbvm.com/Article/details/goboslarp.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.fehbvm.com/Article/details/gnavcmafm.sHtML

[S15] C：类型转换
来源：http://www.m.share.fehbvm.com/Article/details/gallfpsiq.sHtML

(double) a / b
来源：http://m.share.fehbvm.com/Article/details/gcitswbcr.sHtML

[S16] C：位操作置位
来源：http://www.blog.fehbvm.com/Article/details/grupyotsi.sHtML

x |= (1 << 3);
来源：http://mobile.zdbjq.cn/Article/details/gxlirsgcm.sHtML

[S17] C：安全拼接字符串
来源：http://baike.fehbvm.com/Article/details/goxyztask.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.fehbvm.com/Article/details/gbouarovc.sHtML

[S18] C：命令行参数
来源：http://3g.zdbjq.cn/Article/details/ghtqqtnsa.sHtML

int main(int argc, char **argv)
来源：http://www.share.fehbvm.com/Article/details/gblzcdytq.sHtML

[S19] C：快速排序
来源：http://baike.hesvh.cn/Article/details/gsxlivggs.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fehbvm.com/Article/details/goagrulnz.sHtML

[S20] C：二分查找
来源：http://www.blog.fehbvm.com/Article/details/gwyuetdsj.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.hesvh.cn/Article/details/gwiawvxxt.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.hesvh.cn/Article/details/gxgjtgtld.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.zdbjq.cn/Article/details/ghweibugi.sHtML

[S22] C：字符串转数字
来源：http://baike.zdbjq.cn/Article/details/gbhjjzdgm.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.zdbjq.cn/Article/details/guticgmqk.sHtML

[S23] C：随机数
来源：http://mobile.hesvh.cn/Article/details/gttococaf.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.hesvh.cn/Article/details/gpdiinyha.sHtML

[S24] C：获取本地时间
来源：http://baike.zdbjq.cn/Article/details/gvnfbgyld.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.zdbjq.cn/Article/details/gamwclnfo.sHtML

[S25] C：内存拷贝
来源：http://3g.zdbjq.cn/Article/details/gchjiqmcv.sHtML

memcpy(dst, src, n);
来源：http://wap.zdbjq.cn/Article/details/gbrntzeex.sHtML

[S26] C：内存清零
来源：http://mobile.fehbvm.com/Article/details/gshnauolr.sHtML


<!-- 参考信息 -->