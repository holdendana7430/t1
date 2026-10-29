代发 wailian999

[Q44] IN 子查询
来源：http://mobile.zdbjq.cn/Article/details/grizgrchs.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.hesvh.cn/Article/details/gayesxgli.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.fehbvm.com/Article/details/gkgxcmtua.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fehbvm.com/Article/details/gddjvhgfa.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.zdbjq.cn/Article/details/gfaqhrwlw.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fehbvm.com/Article/details/gilbunelf.sHtML

[Q47] 与平均值比较
来源：http://blog.hesvh.cn/Article/details/gammatjmb.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.zdbjq.cn/Article/details/gysiezskw.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.fehbvm.com/Article/details/gqjvhguam.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.zdbjq.cn/Article/details/gylrqydch.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.fehbvm.com/Article/details/garxwwdfm.sHtML

[Q49] 更新单行
来源：http://wap.hesvh.cn/Article/details/gkorhzzvk.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.hesvh.cn/Article/details/gybdopvtd.sHtML

[Q50] 批量更新
来源：http://blog.fehbvm.com/Article/details/girprasgm.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.zdbjq.cn/Article/details/gcxlxluzg.sHtML

[Q51] 用子查询更新
来源：http://blog.fehbvm.com/Article/details/gfqnzalnc.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.hesvh.cn/Article/details/gyqfisxlx.sHtML

[Q52] 删除指定行
来源：http://3g.hesvh.cn/Article/details/gwjpvqegr.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.fehbvm.com/Article/details/grmdckovs.sHtML

[Q53] 按条件删除
来源：http://blog.fehbvm.com/Article/details/gjumpvhze.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.fehbvm.com/Article/details/gicqptelx.sHtML

[Q54] 清空表
来源：http://wap.fehbvm.com/Article/details/gutbsegin.sHtML

TRUNCATE TABLE logs;
来源：http://blog.hesvh.cn/Article/details/giawbfdfw.sHtML

[Q55] 排名（并列占位）
来源：http://blog.hesvh.cn/Article/details/ghrrfarxh.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.zdbjq.cn/Article/details/gkhgwveod.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.zdbjq.cn/Article/details/giivibmfw.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.hesvh.cn/Article/details/gauelycdi.sHtML

[Q57] 行号
来源：http://3g.fehbvm.com/Article/details/gxjssosjb.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gyfwceuig.sHtML

[Q58] 累计求和
来源：http://www.blog.fehbvm.com/Article/details/gywjxrkuo.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.hesvh.cn/Article/details/gfscwizqq.sHtML

[Q59] 分组内累计
来源：http://www.m.share.zdbjq.cn/Article/details/gbgpgjbst.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gomdtbbrj.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.zdbjq.cn/Article/details/grwqblqbk.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.fehbvm.com/Article/details/gcjylfsfy.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.fehbvm.com/Article/details/gaaxwlzbh.sHtML

[Q61] 移动平均
来源：http://m.share.fehbvm.com/Article/details/guvpqorvd.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gsfmnsdqd.sHtML

[Q62] 分组占比
来源：http://mobile.zdbjq.cn/Article/details/gkewxhtor.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.zdbjq.cn/Article/details/gczpapadl.sHtML

[Q63] 开启事务
来源：http://www.share.zdbjq.cn/Article/details/gbeygghnl.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.zdbjq.cn/Article/details/gwbstnpjz.sHtML

[Q64] 提交事务
来源：http://www.share.hesvh.cn/Article/details/gvletvhdu.sHtML

COMMIT;
来源：http://baike.zdbjq.cn/Article/details/geqqxbqrt.sHtML

[Q65] 回滚事务
来源：http://mobile.zdbjq.cn/Article/details/gdwmoyygr.sHtML

ROLLBACK;
来源：http://blog.zdbjq.cn/Article/details/gzugnedop.sHtML

[Q66] 行锁查询
来源：http://blog.hesvh.cn/Article/details/gmjmaxbrt.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.fehbvm.com/Article/details/gweokfgat.sHtML

[Q67] 设置隔离级别
来源：http://baike.zdbjq.cn/Article/details/golkvrnnc.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.fehbvm.com/Article/details/gdqlqxqtr.sHtML

[Q68] 保存点
来源：http://blog.hesvh.cn/Article/details/gpwhmmftp.sHtML

SAVEPOINT sp1;
来源：http://3g.zdbjq.cn/Article/details/gkdyaynua.sHtML

ROLLBACK TO sp1;
来源：http://read.share.zdbjq.cn/Article/details/ganrxssys.sHtML

[Q69] 查看执行计划
来源：http://3g.zdbjq.cn/Article/details/gonuwsogy.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.zdbjq.cn/Article/details/gicnymrnd.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.fehbvm.com/Article/details/gemolpfbm.sHtML

ANALYZE TABLE users;
来源：http://baike.hesvh.cn/Article/details/gqqvnemjr.sHtML

[Q71] 查看建表语句
来源：http://mobile.zdbjq.cn/Article/details/gtuemkyly.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.zdbjq.cn/Article/details/gjmjszyzy.sHtML

[Q72] 查看索引
来源：http://mobile.zdbjq.cn/Article/details/galdsnqev.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gpagmjewy.sHtML

[Q73] 查看表状态
来源：http://wap.fehbvm.com/Article/details/gsziqqdyt.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.hesvh.cn/Article/details/gxddwijbb.sHtML

[Q74] 强制使用索引
来源：http://m.share.hesvh.cn/Article/details/gvzwimolj.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.fehbvm.com/Article/details/geylfkoaf.sHtML

[Q75] 日期格式化
来源：http://blog.fehbvm.com/Article/details/gnookqtck.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gztqnjymb.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.fehbvm.com/Article/details/ggdfqhghu.sHtML

[Q76] 按天统计
来源：http://mobile.zdbjq.cn/Article/details/gppbvkqwx.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.zdbjq.cn/Article/details/gjaxljuxh.sHtML

[Q77] 时间加减
来源：http://read.share.zdbjq.cn/Article/details/gbvhzontv.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.fehbvm.com/Article/details/gyburahrz.sHtML

[Q78] 当前时间
来源：http://3g.fehbvm.com/Article/details/gcrgycflv.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.hesvh.cn/Article/details/gmyclwlcb.sHtML

[Q79] 字符串拼接
来源：http://m.share.zdbjq.cn/Article/details/gzedgjxlx.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.hesvh.cn/Article/details/gyrzsnmwq.sHtML

[Q80] 字符串截取
来源：http://www.blog.hesvh.cn/Article/details/gorofemqn.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.fehbvm.com/Article/details/gzldncjjb.sHtML

[Q81] 字符串替换
来源：http://wap.zdbjq.cn/Article/details/guikkuphb.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.fehbvm.com/Article/details/gbasrbqcl.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.hesvh.cn/Article/details/gercvkgrf.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.hesvh.cn/Article/details/ggozsvsin.sHtML

[Q83] 大小写转换
来源：http://read.share.fehbvm.com/Article/details/gtszdtheo.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gejtxntki.sHtML

[Q84] 去除首尾空格
来源：http://blog.zdbjq.cn/Article/details/gvnyylrng.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/gqkbdyvgo.sHtML

[Q85] 数值取整
来源：http://3g.fehbvm.com/Article/details/gpdwymcth.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.hesvh.cn/Article/details/gkirjxmcl.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.hesvh.cn/Article/details/glohtisib.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.fehbvm.com/Article/details/gslyluchh.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.zdbjq.cn/Article/details/ghgkjxvre.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.fehbvm.com/Article/details/gzlmllzza.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.zdbjq.cn/Article/details/gdwnmxovq.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.fehbvm.com/Article/details/gmiqzzaxy.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.hesvh.cn/Article/details/gsqwjusfp.sHtML

[Q89] 判断表是否存在
来源：http://www.share.hesvh.cn/Article/details/gczmwaopw.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.hesvh.cn/Article/details/gmfweqivj.sHtML

[Q90] 生成序号列
来源：http://www.m.share.fehbvm.com/Article/details/gocoduwuu.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.fehbvm.com/Article/details/ghresihae.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gpyxlvudp.sHtML

R. Bash 专题
来源：http://blog.zdbjq.cn/Article/details/gbfggtnvq.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gtjesfwyg.sHtML

[R01] shebang 与严格模式
来源：http://baike.hesvh.cn/Article/details/gtbpeuuxm.sHtML

#!/usr/bin/env bash
来源：http://mobile.zdbjq.cn/Article/details/gdvzbxlgu.sHtML

set -euo pipefail
来源：http://blog.fehbvm.com/Article/details/gewtzrfwf.sHtML

[R02] 变量赋值与使用
来源：http://blog.fehbvm.com/Article/details/gjodjazwx.sHtML

name="Tom"; echo "$name"
来源：http://baike.hesvh.cn/Article/details/gmkciogtj.sHtML

[R03] 只读变量
来源：http://mobile.hesvh.cn/Article/details/gmqecropf.sHtML

readonly PI=3.14
来源：http://read.share.fehbvm.com/Article/details/grzyblwot.sHtML

[R04] 位置参数
来源：http://www.blog.hesvh.cn/Article/details/gersgvxuo.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.zdbjq.cn/Article/details/gzmvfmrhh.sHtML

[R05] 参数默认值
来源：http://wap.hesvh.cn/Article/details/gsmuzsphv.sHtML

name="${1:-default}"
来源：http://read.share.zdbjq.cn/Article/details/gbyplpcvn.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.hesvh.cn/Article/details/gpeewhrvo.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.hesvh.cn/Article/details/gbpecsuze.sHtML

[R07] if 判断文件
来源：http://wap.zdbjq.cn/Article/details/glmbsksks.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.hesvh.cn/Article/details/gcgknehog.sHtML

[R08] 数值比较
来源：http://wap.fehbvm.com/Article/details/gqwetmugl.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.fehbvm.com/Article/details/gjtksbmxu.sHtML

[R09] 字符串比较
来源：http://m.share.fehbvm.com/Article/details/gpcvrfalr.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.zdbjq.cn/Article/details/giivrdujn.sHtML

[R10] 正则匹配
来源：http://blog.zdbjq.cn/Article/details/gdiaznajo.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.zdbjq.cn/Article/details/gydayhphh.sHtML

[R11] case 多分支
来源：http://www.blog.zdbjq.cn/Article/details/ggxghfejp.sHtML

case "$1" in
来源：http://3g.fehbvm.com/Article/details/gkmcdiewn.sHtML

start) echo "启动" ;;
来源：http://www.share.zdbjq.cn/Article/details/gjgqluxim.sHtML

stop)  echo "停止" ;;
来源：http://baike.fehbvm.com/Article/details/gegnmqdyq.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.hesvh.cn/Article/details/gcuoyqwxm.sHtML

esac
来源：http://www.share.fehbvm.com/Article/details/gouotpfos.sHtML

[R12] for 遍历文件
来源：http://baike.fehbvm.com/Article/details/gllxrxabw.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.fehbvm.com/Article/details/gfvvewzyu.sHtML

[R13] for 计数循环
来源：http://read.share.hesvh.cn/Article/details/gkseoibdc.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.fehbvm.com/Article/details/gaqeedvgu.sHtML

[R14] C 风格 for
来源：http://3g.fehbvm.com/Article/details/gtscxoqtv.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.fehbvm.com/Article/details/gckvxhhks.sHtML

[R15] while 逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gwlipnoij.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.fehbvm.com/Article/details/ggwpdsuik.sHtML

[R16] until 等待条件
来源：http://m.share.zdbjq.cn/Article/details/glamompsy.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.hesvh.cn/Article/details/gggtoexkw.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.hesvh.cn/Article/details/gawrmiypq.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.hesvh.cn/Article/details/gtgwwmcjp.sHtML

[R18] 遍历数组
来源：http://www.m.share.fehbvm.com/Article/details/grljassfd.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.fehbvm.com/Article/details/gbfaevvam.sHtML

[R19] 数组长度
来源：http://baike.zdbjq.cn/Article/details/grrgadtta.sHtML

echo "${#arr[@]}"
来源：http://mobile.zdbjq.cn/Article/details/gehlotnyw.sHtML

[R20] 关联数组（字典）
来源：http://m.share.hesvh.cn/Article/details/gewfojqxr.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.fehbvm.com/Article/details/gxpvlowwf.sHtML

[R21] 字符串长度
来源：http://wap.hesvh.cn/Article/details/gkosnrgmt.sHtML

echo "${#s}"
来源：http://www.share.fehbvm.com/Article/details/glawhirtw.sHtML

[R22] 截取子串
来源：http://wap.zdbjq.cn/Article/details/gvheacuzl.sHtML

echo "${s:0:5}"
来源：http://www.share.zdbjq.cn/Article/details/girxufllp.sHtML

[R23] 字符串替换
来源：http://3g.fehbvm.com/Article/details/ggdnaogsr.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.fehbvm.com/Article/details/gvesusdgt.sHtML

[R24] 大小写转换
来源：http://read.share.fehbvm.com/Article/details/gypxfirxf.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.fehbvm.com/Article/details/gmshgwbow.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.hesvh.cn/Article/details/gjeyjshhu.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.zdbjq.cn/Article/details/gtquqtxkh.sHtML

[R26] 命令替换
来源：http://www.share.zdbjq.cn/Article/details/gwmthfykw.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.fehbvm.com/Article/details/grerpehgc.sHtML

[R27] 算术展开
来源：http://wap.fehbvm.com/Article/details/gbuyegawo.sHtML

echo $((1 + 2 * 3))
来源：http://3g.zdbjq.cn/Article/details/gstkojitd.sHtML

[R28] 浮点运算
来源：http://m.share.hesvh.cn/Article/details/gaomeyutj.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fehbvm.com/Article/details/gtxrloial.sHtML

[R29] 定义函数
来源：http://baike.zdbjq.cn/Article/details/gohihrtgv.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.zdbjq.cn/Article/details/gxtmejpdn.sHtML

[R30] 函数返回状态码
来源：http://blog.fehbvm.com/Article/details/guxhjiwcb.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.fehbvm.com/Article/details/gwyvclwgh.sHtML

[R31] 局部变量
来源：http://wap.zdbjq.cn/Article/details/gzfsgqyqc.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.hesvh.cn/Article/details/gnrvfyhay.sHtML

[R32] 参数个数校验
来源：http://baike.zdbjq.cn/Article/details/gkjnkiqvf.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.hesvh.cn/Article/details/gwovxvkbh.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.fehbvm.com/Article/details/geqispnmx.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.fehbvm.com/Article/details/gsaprzesf.sHtML

[R34] 退出时清理
来源：http://wap.fehbvm.com/Article/details/glhyobkhm.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fehbvm.com/Article/details/gtprfpipl.sHtML

[R35] 后台执行并等待
来源：http://mobile.fehbvm.com/Article/details/gpktsoqay.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.hesvh.cn/Article/details/gxmbawxhi.sHtML

[R36] 并发执行多个任务
来源：http://www.share.zdbjq.cn/Article/details/gtswklyzk.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fehbvm.com/Article/details/gnsfczaru.sHtML

[R37] 把输出赋给变量
来源：http://m.share.fehbvm.com/Article/details/gourukybd.sHtML

files=$(ls -1)
来源：http://www.m.share.zdbjq.cn/Article/details/gxkjfddoe.sHtML

[R38] 管道串联
来源：http://3g.zdbjq.cn/Article/details/gepntwvkl.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fehbvm.com/Article/details/gypmdjaps.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.hesvh.cn/Article/details/gxzdcuhgt.sHtML

cmd > out.log 2>&1
来源：http://wap.hesvh.cn/Article/details/gclepztha.sHtML

[R40] 追加写日志
来源：http://mobile.hesvh.cn/Article/details/grbygzxyw.sHtML

echo "log" >> out.log
来源：http://www.share.hesvh.cn/Article/details/grddfbngb.sHtML

[R41] 丢弃输出
来源：http://www.blog.fehbvm.com/Article/details/gnnsggojg.sHtML

cmd >/dev/null 2>&1
来源：http://3g.hesvh.cn/Article/details/glhgdzayh.sHtML

[R42] 输入重定向
来源：http://m.share.zdbjq.cn/Article/details/gaeyrslkm.sHtML

wc -l < a.txt
来源：http://wap.fehbvm.com/Article/details/gsbbtjzwv.sHtML

[R43] 按名字查找文件
来源：http://blog.hesvh.cn/Article/details/gevukawdj.sHtML

find . -name "*.log" -type f
来源：http://wap.fehbvm.com/Article/details/gufmzfntt.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fehbvm.com/Article/details/gpogozpzd.sHtML

find . -mtime -7 -type f
来源：http://read.share.hesvh.cn/Article/details/gkrnlssmq.sHtML

[R45] 批量删除
来源：http://read.share.hesvh.cn/Article/details/gbjpvghtt.sHtML

find . -name "*.tmp" -delete
来源：http://3g.hesvh.cn/Article/details/gioekljjh.sHtML

[R46] 递归替换文件内容
来源：http://3g.fehbvm.com/Article/details/gggogiklm.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fehbvm.com/Article/details/gsmgzfxlz.sHtML

[R47] sed 单行替换
来源：http://blog.hesvh.cn/Article/details/gjeograxy.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.hesvh.cn/Article/details/guhauqapg.sHtML

[R48] awk 取指定列
来源：http://mobile.fehbvm.com/Article/details/gajfwvapv.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.hesvh.cn/Article/details/guvxbqgrz.sHtML

[R49] awk 带条件
来源：http://www.share.fehbvm.com/Article/details/glfbwnnso.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.hesvh.cn/Article/details/geinksqsm.sHtML

[R50] awk 求和
来源：http://www.m.share.hesvh.cn/Article/details/gemiurlvi.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.hesvh.cn/Article/details/gvwbazpsj.sHtML

[R51] 排序去重取前几
来源：http://baike.hesvh.cn/Article/details/gbyldogai.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fehbvm.com/Article/details/gpbpjtvst.sHtML

[R52] 统计行数
来源：http://wap.fehbvm.com/Article/details/gbvymtipm.sHtML

wc -l a.txt
来源：http://www.blog.zdbjq.cn/Article/details/ggiecxasv.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.zdbjq.cn/Article/details/gzezsgzag.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.zdbjq.cn/Article/details/gppjawevf.sHtML

[R54] 比较两个文件
来源：http://read.share.fehbvm.com/Article/details/gfirqthfg.sHtML

diff a.txt b.txt
来源：http://www.blog.zdbjq.cn/Article/details/gwmzxxvjr.sHtML

[R55] 压缩与解压
来源：http://wap.zdbjq.cn/Article/details/guvataica.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.hesvh.cn/Article/details/gttqxdyum.sHtML

[R56] 远程拷贝
来源：http://www.share.fehbvm.com/Article/details/ggcpqjidy.sHtML

scp file user@host:/path/
来源：http://mobile.fehbvm.com/Article/details/gsfymibxv.sHtML

[R57] 远程执行命令
来源：http://blog.fehbvm.com/Article/details/gyduetkak.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.hesvh.cn/Article/details/gmynjlddw.sHtML

[R58] 下载文件
来源：http://blog.zdbjq.cn/Article/details/gqmaiqzfd.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.zdbjq.cn/Article/details/gkfntdxdx.sHtML

[R59] 发 POST JSON
来源：http://mobile.fehbvm.com/Article/details/gnodbsoyu.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.hesvh.cn/Article/details/gjusgzahy.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.zdbjq.cn/Article/details/gkqcayccv.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.zdbjq.cn/Article/details/gehcazqbl.sHtML

[R61] 磁盘占用
来源：http://www.blog.hesvh.cn/Article/details/gbrcdqaza.sHtML

df -h;  du -sh *
来源：http://blog.zdbjq.cn/Article/details/gvjemmnmf.sHtML

[R62] 找最占空间的文件
来源：http://3g.zdbjq.cn/Article/details/gwofislmj.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.hesvh.cn/Article/details/giifuupxj.sHtML

[R63] 内存与进程
来源：http://www.share.hesvh.cn/Article/details/gpvpykkqf.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.zdbjq.cn/Article/details/guyiabyqw.sHtML

[R64] 结束进程
来源：http://3g.fehbvm.com/Article/details/gqfjtnumu.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.hesvh.cn/Article/details/gkucggmoh.sHtML

[R65] 查看端口占用
来源：http://mobile.zdbjq.cn/Article/details/giebjugrl.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.hesvh.cn/Article/details/gyusmaotu.sHtML

[R66] 定时任务
来源：http://wap.fehbvm.com/Article/details/gaatdqvdn.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.fehbvm.com/Article/details/gpndixsyf.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.zdbjq.cn/Article/details/glllfuoaw.sHtML

openssl rand -hex 16
来源：http://read.share.hesvh.cn/Article/details/gwibtmwod.sHtML

[R68] 计算文件校验值
来源：http://3g.fehbvm.com/Article/details/ggkyrvpwv.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fehbvm.com/Article/details/ghliojptb.sHtML

[R69] 生成随机密码
来源：http://mobile.fehbvm.com/Article/details/gwlsajpse.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fehbvm.com/Article/details/gpaaqnror.sHtML

[R70] 时间戳与互转
来源：http://3g.hesvh.cn/Article/details/gophhulcd.sHtML

date +%s;  date -d @1700000000
来源：http://3g.hesvh.cn/Article/details/gwwjqletk.sHtML

[R71] 日期格式化
来源：http://mobile.fehbvm.com/Article/details/gsonyvlms.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.zdbjq.cn/Article/details/gsqefwlpe.sHtML

[R72] 等待端口就绪
来源：http://www.blog.zdbjq.cn/Article/details/gdzekcjop.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.hesvh.cn/Article/details/ggremdvhk.sHtML

[R73] 分割大日志
来源：http://read.share.zdbjq.cn/Article/details/gfmztpviz.sHtML

split -l 1000 big.log part_
来源：http://wap.fehbvm.com/Article/details/gsvibmiqa.sHtML

[R74] 批量重命名
来源：http://3g.hesvh.cn/Article/details/gnezqbmkt.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fehbvm.com/Article/details/gvrrofhme.sHtML

[R75] 导出环境变量
来源：http://wap.zdbjq.cn/Article/details/gkdvtwyot.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.zdbjq.cn/Article/details/gnenqlbow.sHtML

[R76] 使用临时文件
来源：http://wap.zdbjq.cn/Article/details/gsozqtxyr.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fehbvm.com/Article/details/gspormrdj.sHtML

[R77] 读取用户输入
来源：http://3g.fehbvm.com/Article/details/glllofmzn.sHtML

read -rp "请输入: " ans
来源：http://3g.fehbvm.com/Article/details/gdlsmfdyr.sHtML

[R78] 交互式菜单
来源：http://blog.fehbvm.com/Article/details/gbzrohcfw.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.zdbjq.cn/Article/details/gyrvcogtd.sHtML

[R79] 解析命令行选项
来源：http://read.share.hesvh.cn/Article/details/gzyegrlch.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.hesvh.cn/Article/details/gmhfhlght.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.hesvh.cn/Article/details/gbwoiqdfo.sHtML

time ./run.sh
来源：http://blog.fehbvm.com/Article/details/gaimnrabz.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gvlnkxqxs.sHtML

S. C / C++ 专题
来源：http://www.m.share.zdbjq.cn/Article/details/gokopupgw.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gsveogpxn.sHtML

[S01] C：Hello World
来源：http://mobile.hesvh.cn/Article/details/gdffmfzub.sHtML

#include <stdio.h>
来源：http://read.share.hesvh.cn/Article/details/grzdvqxaw.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.hesvh.cn/Article/details/gxmkhxtkt.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.hesvh.cn/Article/details/gctaooery.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.hesvh.cn/Article/details/gyerdfmzf.sHtML

[S03] C：读入整数
来源：http://3g.zdbjq.cn/Article/details/gsllpqtsg.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.hesvh.cn/Article/details/gxazfcolj.sHtML

[S04] C：字符串复制
来源：http://3g.hesvh.cn/Article/details/gzwiluycd.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.fehbvm.com/Article/details/gmfncrvlc.sHtML

[S05] C：字符串长度
来源：http://blog.hesvh.cn/Article/details/gnkzxeqcm.sHtML

strlen(s)
来源：http://www.blog.zdbjq.cn/Article/details/gjhhlqedz.sHtML

[S06] C：字符串比较
来源：http://www.blog.zdbjq.cn/Article/details/gkyikkvzz.sHtML

strcmp(a, b) == 0
来源：http://www.share.fehbvm.com/Article/details/gxoyxbrqd.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.hesvh.cn/Article/details/gyzunjcho.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.hesvh.cn/Article/details/gzstnmcix.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.hesvh.cn/Article/details/gfcxzqtzr.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.hesvh.cn/Article/details/gavgevgqb.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.hesvh.cn/Article/details/gwpdwlwcr.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.fehbvm.com/Article/details/getmlpuzh.sHtML

[S10] C：指针与解引用
来源：http://read.share.fehbvm.com/Article/details/gwcbfmphw.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fehbvm.com/Article/details/gvwybugym.sHtML

[S11] C：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gqoctkzmp.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.fehbvm.com/Article/details/gvtgvvtnl.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.fehbvm.com/Article/details/gktjsntyw.sHtML

fclose(f);
来源：http://3g.zdbjq.cn/Article/details/gbsbhgcvf.sHtML

[S12] C：写文件
来源：http://3g.zdbjq.cn/Article/details/gkikdnima.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.fehbvm.com/Article/details/gghizyruy.sHtML

[S13] C：宏定义
来源：http://3g.fehbvm.com/Article/details/gjttargpp.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fehbvm.com/Article/details/gddyozwfy.sHtML

[S14] C：枚举
来源：http://blog.zdbjq.cn/Article/details/gzrqofarr.sHtML


<!-- 参考信息 -->