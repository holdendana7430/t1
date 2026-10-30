代发 wailian999

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.fehbvm.com/Article/details/gjbhkklnh.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.zdbjq.cn/Article/details/glzamwesq.sHtML

[Q47] 与平均值比较
来源：http://wap.zdbjq.cn/Article/details/gdfixuhlw.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.hesvh.cn/Article/details/gekpznuep.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.hesvh.cn/Article/details/gmidlktta.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.hesvh.cn/Article/details/gwzgondga.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.hesvh.cn/Article/details/gvwncmbep.sHtML

[Q49] 更新单行
来源：http://mobile.zdbjq.cn/Article/details/gushltmsp.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.hesvh.cn/Article/details/gyeszmknr.sHtML

[Q50] 批量更新
来源：http://m.share.hesvh.cn/Article/details/ggdjkbutk.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.hesvh.cn/Article/details/gseaqcuin.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.zdbjq.cn/Article/details/gompjpiwh.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.fehbvm.com/Article/details/geqgvadtk.sHtML

[Q52] 删除指定行
来源：http://3g.zdbjq.cn/Article/details/ghzssfnzs.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gerifurjz.sHtML

[Q53] 按条件删除
来源：http://3g.zdbjq.cn/Article/details/gxansardf.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.zdbjq.cn/Article/details/glcjilahr.sHtML

[Q54] 清空表
来源：http://www.blog.zdbjq.cn/Article/details/gyongullk.sHtML

TRUNCATE TABLE logs;
来源：http://3g.fehbvm.com/Article/details/gkdjhzpcx.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.zdbjq.cn/Article/details/glwzblmsp.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.zdbjq.cn/Article/details/gfnnfazwr.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.fehbvm.com/Article/details/gzsuqfncv.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.fehbvm.com/Article/details/gmwdguypu.sHtML

[Q57] 行号
来源：http://read.share.zdbjq.cn/Article/details/gzgxeiwdd.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gfcchuqhr.sHtML

[Q58] 累计求和
来源：http://blog.zdbjq.cn/Article/details/gtbhbndyb.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.fehbvm.com/Article/details/goucijsjd.sHtML

[Q59] 分组内累计
来源：http://blog.zdbjq.cn/Article/details/gorhnozxy.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gqcvdrebo.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.hesvh.cn/Article/details/gmqvadtre.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.zdbjq.cn/Article/details/gzkwuofoe.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gkqpwaaod.sHtML

[Q61] 移动平均
来源：http://m.share.zdbjq.cn/Article/details/ggnxricnx.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gjwsfnfva.sHtML

[Q62] 分组占比
来源：http://www.share.hesvh.cn/Article/details/gmifdpwsj.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.zdbjq.cn/Article/details/gybpliaar.sHtML

[Q63] 开启事务
来源：http://mobile.fehbvm.com/Article/details/gnlvmjrrm.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.hesvh.cn/Article/details/gewjgefau.sHtML

[Q64] 提交事务
来源：http://baike.hesvh.cn/Article/details/gxuidtpgb.sHtML

COMMIT;
来源：http://baike.hesvh.cn/Article/details/guawputrx.sHtML

[Q65] 回滚事务
来源：http://www.blog.zdbjq.cn/Article/details/gffibdjoc.sHtML

ROLLBACK;
来源：http://mobile.hesvh.cn/Article/details/galioybcv.sHtML

[Q66] 行锁查询
来源：http://3g.zdbjq.cn/Article/details/gxkoercfw.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.fehbvm.com/Article/details/gryijmeeo.sHtML

[Q67] 设置隔离级别
来源：http://baike.fehbvm.com/Article/details/gjgigwgot.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.zdbjq.cn/Article/details/gcjujhcad.sHtML

[Q68] 保存点
来源：http://www.m.share.hesvh.cn/Article/details/ggxtyfsnd.sHtML

SAVEPOINT sp1;
来源：http://baike.fehbvm.com/Article/details/gdcfzeyqi.sHtML

ROLLBACK TO sp1;
来源：http://read.share.hesvh.cn/Article/details/gftulhuak.sHtML

[Q69] 查看执行计划
来源：http://blog.zdbjq.cn/Article/details/gzpbqdkqz.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.fehbvm.com/Article/details/gygopvxqk.sHtML

[Q70] 更新统计信息
来源：http://3g.zdbjq.cn/Article/details/gblbxwicf.sHtML

ANALYZE TABLE users;
来源：http://3g.fehbvm.com/Article/details/gwmhoqqsz.sHtML

[Q71] 查看建表语句
来源：http://www.share.hesvh.cn/Article/details/gjkagjldm.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.zdbjq.cn/Article/details/gasnvsxxu.sHtML

[Q72] 查看索引
来源：http://www.blog.hesvh.cn/Article/details/ggfckiolf.sHtML

SHOW INDEX FROM users;
来源：http://m.share.zdbjq.cn/Article/details/guispmkuz.sHtML

[Q73] 查看表状态
来源：http://3g.zdbjq.cn/Article/details/gsacwngup.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.fehbvm.com/Article/details/gbasefpwq.sHtML

[Q74] 强制使用索引
来源：http://m.share.hesvh.cn/Article/details/gndbciajf.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.hesvh.cn/Article/details/gynpxgfrm.sHtML

[Q75] 日期格式化
来源：http://wap.zdbjq.cn/Article/details/gqnmbjnnl.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.hesvh.cn/Article/details/gvfznhfzy.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.hesvh.cn/Article/details/guhpueegl.sHtML

[Q76] 按天统计
来源：http://blog.zdbjq.cn/Article/details/ghdabgmnz.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.fehbvm.com/Article/details/gooamgwnv.sHtML

[Q77] 时间加减
来源：http://wap.zdbjq.cn/Article/details/gfrdiosln.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.zdbjq.cn/Article/details/gaghelllm.sHtML

[Q78] 当前时间
来源：http://www.share.zdbjq.cn/Article/details/gykmxymvo.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.hesvh.cn/Article/details/gqoheofcg.sHtML

[Q79] 字符串拼接
来源：http://www.share.hesvh.cn/Article/details/gnvwqriyy.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.zdbjq.cn/Article/details/gufmeqjnk.sHtML

[Q80] 字符串截取
来源：http://m.share.hesvh.cn/Article/details/geitshsso.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gkztkmnlr.sHtML

[Q81] 字符串替换
来源：http://read.share.hesvh.cn/Article/details/gmqgkapdz.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.zdbjq.cn/Article/details/gvwtrhkwp.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.fehbvm.com/Article/details/gmqmetnkc.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gzzmmffcd.sHtML

[Q83] 大小写转换
来源：http://mobile.zdbjq.cn/Article/details/gunphigos.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/grtzyawab.sHtML

[Q84] 去除首尾空格
来源：http://mobile.fehbvm.com/Article/details/gruuqznsh.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gmztahpkx.sHtML

[Q85] 数值取整
来源：http://www.m.share.fehbvm.com/Article/details/gamlkjewk.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.hesvh.cn/Article/details/gscibqyyg.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.hesvh.cn/Article/details/gshniiufc.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.fehbvm.com/Article/details/gsayzqxgv.sHtML

[Q87] JSON 字段做条件
来源：http://3g.hesvh.cn/Article/details/gnwdsuvfc.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.fehbvm.com/Article/details/gwitofmdm.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.zdbjq.cn/Article/details/gnvxlzvop.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.fehbvm.com/Article/details/geprwcram.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.hesvh.cn/Article/details/gauubtusl.sHtML

[Q89] 判断表是否存在
来源：http://read.share.zdbjq.cn/Article/details/glhkjnbgj.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.fehbvm.com/Article/details/gusewltov.sHtML

[Q90] 生成序号列
来源：http://www.blog.fehbvm.com/Article/details/gylxinpkn.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.zdbjq.cn/Article/details/gzathifhq.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gxypjduzk.sHtML

R. Bash 专题
来源：http://m.share.zdbjq.cn/Article/details/gwvjhunbk.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gqyllnssu.sHtML

[R01] shebang 与严格模式
来源：http://www.share.zdbjq.cn/Article/details/gzxqmqxwv.sHtML

#!/usr/bin/env bash
来源：http://wap.fehbvm.com/Article/details/gjdiexrvz.sHtML

set -euo pipefail
来源：http://www.m.share.zdbjq.cn/Article/details/gissmrgbm.sHtML

[R02] 变量赋值与使用
来源：http://3g.zdbjq.cn/Article/details/gaahvojja.sHtML

name="Tom"; echo "$name"
来源：http://baike.zdbjq.cn/Article/details/grtogixbk.sHtML

[R03] 只读变量
来源：http://www.m.share.zdbjq.cn/Article/details/gcqvgzbod.sHtML

readonly PI=3.14
来源：http://m.share.zdbjq.cn/Article/details/gumzbffnk.sHtML

[R04] 位置参数
来源：http://wap.hesvh.cn/Article/details/gnstpwjeo.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.fehbvm.com/Article/details/gnxocrifn.sHtML

[R05] 参数默认值
来源：http://baike.hesvh.cn/Article/details/grnrgeohc.sHtML

name="${1:-default}"
来源：http://www.share.hesvh.cn/Article/details/grzppxoai.sHtML

[R06] 判断命令是否存在
来源：http://www.share.fehbvm.com/Article/details/gvlojkpds.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.fehbvm.com/Article/details/grqniukod.sHtML

[R07] if 判断文件
来源：http://3g.fehbvm.com/Article/details/gjaedqxva.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gcpiilvhm.sHtML

[R08] 数值比较
来源：http://mobile.zdbjq.cn/Article/details/gduyrhbih.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.fehbvm.com/Article/details/gdpannark.sHtML

[R09] 字符串比较
来源：http://www.m.share.zdbjq.cn/Article/details/ghlhmfewt.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.hesvh.cn/Article/details/gidagmunh.sHtML

[R10] 正则匹配
来源：http://www.share.hesvh.cn/Article/details/gfladwyja.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.zdbjq.cn/Article/details/giwgvhgsy.sHtML

[R11] case 多分支
来源：http://www.share.hesvh.cn/Article/details/gjpjoqdqc.sHtML

case "$1" in
来源：http://www.share.hesvh.cn/Article/details/ghgznfmzo.sHtML

start) echo "启动" ;;
来源：http://blog.fehbvm.com/Article/details/gmjfdhtsh.sHtML

stop)  echo "停止" ;;
来源：http://read.share.hesvh.cn/Article/details/gtafftjlt.sHtML

*)     echo "未知命令" ;;
来源：http://blog.fehbvm.com/Article/details/girdhdvaz.sHtML

esac
来源：http://blog.hesvh.cn/Article/details/gjgpotjjd.sHtML

[R12] for 遍历文件
来源：http://wap.hesvh.cn/Article/details/grmjucduf.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.zdbjq.cn/Article/details/giosgdymq.sHtML

[R13] for 计数循环
来源：http://www.m.share.zdbjq.cn/Article/details/gpdthdsrv.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.hesvh.cn/Article/details/gmfuvobny.sHtML

[R14] C 风格 for
来源：http://mobile.fehbvm.com/Article/details/glawppjxl.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.fehbvm.com/Article/details/gbalcvgfo.sHtML

[R15] while 逐行读文件
来源：http://read.share.fehbvm.com/Article/details/glvwhosxs.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.zdbjq.cn/Article/details/gmagwuxqc.sHtML

[R16] until 等待条件
来源：http://www.share.hesvh.cn/Article/details/gynoynbxa.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.hesvh.cn/Article/details/gvxgbucdu.sHtML

[R17] 数组定义与取值
来源：http://mobile.fehbvm.com/Article/details/glawpfkao.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.zdbjq.cn/Article/details/ghekrlucg.sHtML

[R18] 遍历数组
来源：http://mobile.hesvh.cn/Article/details/gpybpftvg.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.fehbvm.com/Article/details/golohmseq.sHtML

[R19] 数组长度
来源：http://blog.fehbvm.com/Article/details/gbzculluz.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.hesvh.cn/Article/details/gvkgbxypz.sHtML

[R20] 关联数组（字典）
来源：http://mobile.hesvh.cn/Article/details/gwnvvnovp.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.zdbjq.cn/Article/details/gekakfcpk.sHtML

[R21] 字符串长度
来源：http://3g.hesvh.cn/Article/details/gddnmkcfx.sHtML

echo "${#s}"
来源：http://mobile.zdbjq.cn/Article/details/gteabeusf.sHtML

[R22] 截取子串
来源：http://mobile.hesvh.cn/Article/details/gqlruqknf.sHtML

echo "${s:0:5}"
来源：http://www.blog.fehbvm.com/Article/details/gmshouzni.sHtML

[R23] 字符串替换
来源：http://read.share.fehbvm.com/Article/details/galjwmqmo.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.zdbjq.cn/Article/details/gwqifbrut.sHtML

[R24] 大小写转换
来源：http://blog.fehbvm.com/Article/details/gqqcvkosw.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.hesvh.cn/Article/details/giahpidfc.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.hesvh.cn/Article/details/gluymhlpx.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.fehbvm.com/Article/details/guoffedtw.sHtML

[R26] 命令替换
来源：http://baike.fehbvm.com/Article/details/gjdckhbrf.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.hesvh.cn/Article/details/guxgfmnxg.sHtML

[R27] 算术展开
来源：http://blog.zdbjq.cn/Article/details/gwathdnpx.sHtML

echo $((1 + 2 * 3))
来源：http://wap.zdbjq.cn/Article/details/guuuikell.sHtML

[R28] 浮点运算
来源：http://baike.fehbvm.com/Article/details/gsnfnzydp.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.zdbjq.cn/Article/details/giwmrbmxc.sHtML

[R29] 定义函数
来源：http://www.m.share.fehbvm.com/Article/details/gfqsljdef.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.hesvh.cn/Article/details/gngyoisrc.sHtML

[R30] 函数返回状态码
来源：http://baike.zdbjq.cn/Article/details/gguhymrok.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.hesvh.cn/Article/details/gjfqxupkl.sHtML

[R31] 局部变量
来源：http://3g.zdbjq.cn/Article/details/grqtqhygj.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.zdbjq.cn/Article/details/gcbbqwspj.sHtML

[R32] 参数个数校验
来源：http://read.share.hesvh.cn/Article/details/gusjfrxkq.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.zdbjq.cn/Article/details/gzbtbriaq.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.zdbjq.cn/Article/details/gozdchzss.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.fehbvm.com/Article/details/gcuqjbjjm.sHtML

[R34] 退出时清理
来源：http://3g.fehbvm.com/Article/details/gobivjzhc.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.hesvh.cn/Article/details/gfujcrpim.sHtML

[R35] 后台执行并等待
来源：http://blog.zdbjq.cn/Article/details/grtewxfrj.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.zdbjq.cn/Article/details/gwyrihwmi.sHtML

[R36] 并发执行多个任务
来源：http://3g.zdbjq.cn/Article/details/gaxbejwsi.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.zdbjq.cn/Article/details/gurdfbgqt.sHtML

[R37] 把输出赋给变量
来源：http://wap.hesvh.cn/Article/details/gplgisqna.sHtML

files=$(ls -1)
来源：http://mobile.fehbvm.com/Article/details/guegvjzqb.sHtML

[R38] 管道串联
来源：http://m.share.fehbvm.com/Article/details/gelcfamqs.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fehbvm.com/Article/details/ggzcrgzff.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.hesvh.cn/Article/details/gcfjjfvxg.sHtML

cmd > out.log 2>&1
来源：http://m.share.zdbjq.cn/Article/details/gkgmkogxx.sHtML

[R40] 追加写日志
来源：http://read.share.zdbjq.cn/Article/details/gnreczebh.sHtML

echo "log" >> out.log
来源：http://blog.zdbjq.cn/Article/details/grtuoyaun.sHtML

[R41] 丢弃输出
来源：http://www.m.share.fehbvm.com/Article/details/gqqhucsdy.sHtML

cmd >/dev/null 2>&1
来源：http://wap.fehbvm.com/Article/details/gusziqtyo.sHtML

[R42] 输入重定向
来源：http://read.share.fehbvm.com/Article/details/gdoflqbeh.sHtML

wc -l < a.txt
来源：http://www.share.hesvh.cn/Article/details/gicvcsgzy.sHtML

[R43] 按名字查找文件
来源：http://read.share.zdbjq.cn/Article/details/glscvapsd.sHtML

find . -name "*.log" -type f
来源：http://read.share.zdbjq.cn/Article/details/gxrfxpecr.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fehbvm.com/Article/details/gmegfmwtb.sHtML

find . -mtime -7 -type f
来源：http://www.share.hesvh.cn/Article/details/giqzwspoi.sHtML

[R45] 批量删除
来源：http://blog.fehbvm.com/Article/details/gnpiatqbt.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.fehbvm.com/Article/details/gqwfsuako.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fehbvm.com/Article/details/gmnmtfccp.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.hesvh.cn/Article/details/gztlghrjx.sHtML

[R47] sed 单行替换
来源：http://blog.fehbvm.com/Article/details/gnbrbmiob.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.hesvh.cn/Article/details/guatchxle.sHtML

[R48] awk 取指定列
来源：http://wap.fehbvm.com/Article/details/gvaiksjey.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.fehbvm.com/Article/details/gvdffzcox.sHtML

[R49] awk 带条件
来源：http://blog.hesvh.cn/Article/details/gefmckaqd.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.hesvh.cn/Article/details/ghpbwctvg.sHtML

[R50] awk 求和
来源：http://mobile.zdbjq.cn/Article/details/gkfqlsdjx.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.zdbjq.cn/Article/details/gtoywcqfq.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.zdbjq.cn/Article/details/gyxgvbyba.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.hesvh.cn/Article/details/gptfkohta.sHtML

[R52] 统计行数
来源：http://3g.hesvh.cn/Article/details/glmwkzdwq.sHtML

wc -l a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gcafpunkc.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.hesvh.cn/Article/details/gkopfwfzv.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fehbvm.com/Article/details/gxfcumgio.sHtML

[R54] 比较两个文件
来源：http://wap.zdbjq.cn/Article/details/gucsvyctd.sHtML

diff a.txt b.txt
来源：http://www.m.share.fehbvm.com/Article/details/gvgilshcw.sHtML

[R55] 压缩与解压
来源：http://www.share.zdbjq.cn/Article/details/gnyummqiv.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.zdbjq.cn/Article/details/genzkytut.sHtML

[R56] 远程拷贝
来源：http://www.m.share.hesvh.cn/Article/details/gfrtpoaay.sHtML

scp file user@host:/path/
来源：http://www.share.hesvh.cn/Article/details/gpahmgdlp.sHtML

[R57] 远程执行命令
来源：http://www.share.zdbjq.cn/Article/details/gctzozvwu.sHtML

ssh user@host 'uptime'
来源：http://read.share.hesvh.cn/Article/details/gieepvpgn.sHtML

[R58] 下载文件
来源：http://read.share.fehbvm.com/Article/details/grxuxvtrc.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.zdbjq.cn/Article/details/giemflhet.sHtML

[R59] 发 POST JSON
来源：http://read.share.fehbvm.com/Article/details/gmrybqsiy.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fehbvm.com/Article/details/ghtlfnsmh.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.zdbjq.cn/Article/details/gwefznsfr.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.fehbvm.com/Article/details/gfambztpo.sHtML

[R61] 磁盘占用
来源：http://m.share.hesvh.cn/Article/details/gfnnxymop.sHtML

df -h;  du -sh *
来源：http://mobile.hesvh.cn/Article/details/glounjxft.sHtML

[R62] 找最占空间的文件
来源：http://m.share.hesvh.cn/Article/details/glujxdcxt.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.zdbjq.cn/Article/details/gupbpjwsn.sHtML

[R63] 内存与进程
来源：http://blog.fehbvm.com/Article/details/gvehotsvq.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.zdbjq.cn/Article/details/gmsbbpcbh.sHtML

[R64] 结束进程
来源：http://mobile.zdbjq.cn/Article/details/gpmgobjnc.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.fehbvm.com/Article/details/gpbgqhqki.sHtML

[R65] 查看端口占用
来源：http://3g.hesvh.cn/Article/details/gfhghvkrj.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.fehbvm.com/Article/details/gzsuwbkca.sHtML

[R66] 定时任务
来源：http://m.share.zdbjq.cn/Article/details/gmbfkndev.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.zdbjq.cn/Article/details/gkllaiqzf.sHtML

[R67] 生成随机十六进制串
来源：http://blog.hesvh.cn/Article/details/gjwuywguf.sHtML

openssl rand -hex 16
来源：http://mobile.zdbjq.cn/Article/details/gdeldggqc.sHtML

[R68] 计算文件校验值
来源：http://blog.fehbvm.com/Article/details/gvdkqtvei.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.zdbjq.cn/Article/details/gqczdeasf.sHtML

[R69] 生成随机密码
来源：http://www.m.share.zdbjq.cn/Article/details/gufefvwip.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fehbvm.com/Article/details/goreolruc.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.zdbjq.cn/Article/details/gehdjxobx.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fehbvm.com/Article/details/gsxqgmiuv.sHtML

[R71] 日期格式化
来源：http://www.blog.hesvh.cn/Article/details/gaqrbbczs.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.hesvh.cn/Article/details/guyyslyua.sHtML

[R72] 等待端口就绪
来源：http://baike.hesvh.cn/Article/details/gppoaknrh.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.zdbjq.cn/Article/details/gcuczcvwt.sHtML

[R73] 分割大日志
来源：http://read.share.fehbvm.com/Article/details/gryqyqjla.sHtML

split -l 1000 big.log part_
来源：http://mobile.zdbjq.cn/Article/details/gvenaywfa.sHtML

[R74] 批量重命名
来源：http://www.blog.fehbvm.com/Article/details/gkmwyboqe.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.hesvh.cn/Article/details/ghvriqaiu.sHtML

[R75] 导出环境变量
来源：http://3g.zdbjq.cn/Article/details/gutvpkxga.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.hesvh.cn/Article/details/ghqhbmorv.sHtML

[R76] 使用临时文件
来源：http://baike.fehbvm.com/Article/details/gykzozcxm.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.zdbjq.cn/Article/details/genktjrix.sHtML

[R77] 读取用户输入
来源：http://baike.fehbvm.com/Article/details/gzodcqlgg.sHtML

read -rp "请输入: " ans
来源：http://blog.zdbjq.cn/Article/details/gtwdzexco.sHtML

[R78] 交互式菜单
来源：http://read.share.hesvh.cn/Article/details/gwjmcoaxf.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.hesvh.cn/Article/details/gczoermlk.sHtML

[R79] 解析命令行选项
来源：http://m.share.hesvh.cn/Article/details/gqqvpjzjv.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.zdbjq.cn/Article/details/guoxawqla.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.zdbjq.cn/Article/details/gescnujqf.sHtML

time ./run.sh
来源：http://blog.zdbjq.cn/Article/details/gcxcuogqh.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gpyaxugxi.sHtML

S. C / C++ 专题
来源：http://blog.fehbvm.com/Article/details/gclhnbjzr.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gcxiuedbc.sHtML

[S01] C：Hello World
来源：http://baike.zdbjq.cn/Article/details/gflmjxmvm.sHtML

#include <stdio.h>
来源：http://baike.zdbjq.cn/Article/details/gkpbdwtax.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.zdbjq.cn/Article/details/gmhdsrbma.sHtML

[S02] C：变量与格式化输出
来源：http://blog.hesvh.cn/Article/details/gnouzkyqa.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.zdbjq.cn/Article/details/gbjvzybsb.sHtML

[S03] C：读入整数
来源：http://wap.fehbvm.com/Article/details/glmzfsity.sHtML

int x; scanf("%d", &x);
来源：http://3g.fehbvm.com/Article/details/gxqrquljo.sHtML

[S04] C：字符串复制
来源：http://baike.zdbjq.cn/Article/details/gcpitiwsj.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fehbvm.com/Article/details/gxxuivjlq.sHtML

[S05] C：字符串长度
来源：http://www.m.share.hesvh.cn/Article/details/gnjrysxhx.sHtML

strlen(s)
来源：http://www.m.share.fehbvm.com/Article/details/gnnpbmdvo.sHtML

[S06] C：字符串比较
来源：http://3g.fehbvm.com/Article/details/gdobqulge.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.hesvh.cn/Article/details/gkufizukl.sHtML

[S07] C：数组遍历求和
来源：http://m.share.zdbjq.cn/Article/details/gnhracxjh.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.hesvh.cn/Article/details/gevxiliuz.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.zdbjq.cn/Article/details/gfiznldpw.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.fehbvm.com/Article/details/glgzjurgd.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.hesvh.cn/Article/details/goebduqdt.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.hesvh.cn/Article/details/gsvcaqyhr.sHtML

[S10] C：指针与解引用
来源：http://baike.zdbjq.cn/Article/details/gcvjevfxc.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.zdbjq.cn/Article/details/gadjkrgik.sHtML

[S11] C：逐行读文件
来源：http://baike.fehbvm.com/Article/details/gphsfhkyz.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.hesvh.cn/Article/details/gwkegkqyb.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.hesvh.cn/Article/details/gedkjsify.sHtML

fclose(f);
来源：http://mobile.hesvh.cn/Article/details/gtgrbozpd.sHtML

[S12] C：写文件
来源：http://www.m.share.fehbvm.com/Article/details/gpzxtqmxt.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fehbvm.com/Article/details/gmausecef.sHtML

[S13] C：宏定义
来源：http://www.m.share.hesvh.cn/Article/details/gxorwowtr.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.zdbjq.cn/Article/details/glzduvulo.sHtML

[S14] C：枚举
来源：http://wap.zdbjq.cn/Article/details/gbvvukblx.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.fehbvm.com/Article/details/gsvuvlucl.sHtML

[S15] C：类型转换
来源：http://read.share.fehbvm.com/Article/details/gbyuagzxi.sHtML

(double) a / b
来源：http://m.share.hesvh.cn/Article/details/gnrmqmbld.sHtML

[S16] C：位操作置位
来源：http://3g.zdbjq.cn/Article/details/gavdokrof.sHtML


<!-- 参考信息 -->