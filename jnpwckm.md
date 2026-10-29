代发 wailian999

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.hesvh.cn/Article/details/gnmpysozs.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.zdbjq.cn/Article/details/gtqrrdtsu.sHtML

[Q47] 与平均值比较
来源：http://3g.hesvh.cn/Article/details/gslhtwcto.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.hesvh.cn/Article/details/gwewsubqm.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.zdbjq.cn/Article/details/gltnngqon.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.zdbjq.cn/Article/details/gcabzcnnp.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.fehbvm.com/Article/details/gofavmpny.sHtML

[Q49] 更新单行
来源：http://read.share.fehbvm.com/Article/details/gkeuikcub.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.hesvh.cn/Article/details/gkrayrurr.sHtML

[Q50] 批量更新
来源：http://www.blog.hesvh.cn/Article/details/gerxzcdyu.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.fehbvm.com/Article/details/gfsxnpywf.sHtML

[Q51] 用子查询更新
来源：http://m.share.zdbjq.cn/Article/details/gxcpdhyba.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.hesvh.cn/Article/details/ggorczjbj.sHtML

[Q52] 删除指定行
来源：http://m.share.zdbjq.cn/Article/details/gipytmxkt.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.fehbvm.com/Article/details/gxrswblkj.sHtML

[Q53] 按条件删除
来源：http://wap.fehbvm.com/Article/details/gcxuiseri.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.zdbjq.cn/Article/details/gnelccgcw.sHtML

[Q54] 清空表
来源：http://www.m.share.fehbvm.com/Article/details/gfzsckpdp.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.fehbvm.com/Article/details/gnbbmvebu.sHtML

[Q55] 排名（并列占位）
来源：http://baike.fehbvm.com/Article/details/gzjaqcfnm.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.zdbjq.cn/Article/details/grsnoaqtf.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.zdbjq.cn/Article/details/gitwejtrs.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.zdbjq.cn/Article/details/ghozqcfvc.sHtML

[Q57] 行号
来源：http://wap.fehbvm.com/Article/details/gyvnchdup.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.fehbvm.com/Article/details/gcmxesfby.sHtML

[Q58] 累计求和
来源：http://www.m.share.zdbjq.cn/Article/details/guaqhdrvk.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.hesvh.cn/Article/details/gdsykiofb.sHtML

[Q59] 分组内累计
来源：http://www.share.fehbvm.com/Article/details/gptxeeblc.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.fehbvm.com/Article/details/guzcyxwjy.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.hesvh.cn/Article/details/gzvmvmlbe.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.hesvh.cn/Article/details/gxturiivm.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gyztlroeo.sHtML

[Q61] 移动平均
来源：http://baike.hesvh.cn/Article/details/gpbloyqds.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/ghnlcoloz.sHtML

[Q62] 分组占比
来源：http://m.share.hesvh.cn/Article/details/gsxgmngdv.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.hesvh.cn/Article/details/ghajonnxy.sHtML

[Q63] 开启事务
来源：http://blog.hesvh.cn/Article/details/gafhslfaf.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.fehbvm.com/Article/details/gjzjfvxev.sHtML

[Q64] 提交事务
来源：http://blog.fehbvm.com/Article/details/gschhapbp.sHtML

COMMIT;
来源：http://3g.fehbvm.com/Article/details/gdhfgiarr.sHtML

[Q65] 回滚事务
来源：http://m.share.fehbvm.com/Article/details/gaxfouatz.sHtML

ROLLBACK;
来源：http://read.share.hesvh.cn/Article/details/gojzldthf.sHtML

[Q66] 行锁查询
来源：http://www.blog.zdbjq.cn/Article/details/gscunecfi.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.zdbjq.cn/Article/details/goemvjhqi.sHtML

[Q67] 设置隔离级别
来源：http://blog.hesvh.cn/Article/details/gjpemzlsi.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.hesvh.cn/Article/details/gqmxypqjd.sHtML

[Q68] 保存点
来源：http://www.share.zdbjq.cn/Article/details/gubojxyra.sHtML

SAVEPOINT sp1;
来源：http://mobile.hesvh.cn/Article/details/gluaixkbp.sHtML

ROLLBACK TO sp1;
来源：http://baike.fehbvm.com/Article/details/gyliyjtkr.sHtML

[Q69] 查看执行计划
来源：http://read.share.zdbjq.cn/Article/details/gjyvuceqj.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.zdbjq.cn/Article/details/gttjhqhxh.sHtML

[Q70] 更新统计信息
来源：http://3g.hesvh.cn/Article/details/gkqhxomwk.sHtML

ANALYZE TABLE users;
来源：http://mobile.zdbjq.cn/Article/details/gyfkdohdx.sHtML

[Q71] 查看建表语句
来源：http://read.share.zdbjq.cn/Article/details/gstuljdib.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.zdbjq.cn/Article/details/gilbtxzan.sHtML

[Q72] 查看索引
来源：http://baike.zdbjq.cn/Article/details/gqtjkkwnp.sHtML

SHOW INDEX FROM users;
来源：http://read.share.fehbvm.com/Article/details/gndidxpsf.sHtML

[Q73] 查看表状态
来源：http://3g.fehbvm.com/Article/details/glcqiokgs.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.hesvh.cn/Article/details/ghnhrevgp.sHtML

[Q74] 强制使用索引
来源：http://baike.hesvh.cn/Article/details/gjjizcpqy.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.hesvh.cn/Article/details/gyiwpgxhe.sHtML

[Q75] 日期格式化
来源：http://3g.hesvh.cn/Article/details/gvbomiwix.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.hesvh.cn/Article/details/gngyujgub.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.zdbjq.cn/Article/details/gjsaxwrlr.sHtML

[Q76] 按天统计
来源：http://baike.zdbjq.cn/Article/details/gqhrhoxww.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.fehbvm.com/Article/details/gxpuijttj.sHtML

[Q77] 时间加减
来源：http://m.share.zdbjq.cn/Article/details/gcnuzwuny.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.zdbjq.cn/Article/details/gdkaqcddu.sHtML

[Q78] 当前时间
来源：http://www.m.share.zdbjq.cn/Article/details/gridfaheo.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.zdbjq.cn/Article/details/gcuieaejt.sHtML

[Q79] 字符串拼接
来源：http://3g.fehbvm.com/Article/details/gabjnjaup.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.zdbjq.cn/Article/details/gposwoned.sHtML

[Q80] 字符串截取
来源：http://baike.hesvh.cn/Article/details/gwfyjicrs.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gfubqztdb.sHtML

[Q81] 字符串替换
来源：http://www.m.share.hesvh.cn/Article/details/gukzmxcgf.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gliigjdus.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.fehbvm.com/Article/details/gwnmjvylv.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/ggluwxyfo.sHtML

[Q83] 大小写转换
来源：http://www.m.share.zdbjq.cn/Article/details/ggiambako.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.hesvh.cn/Article/details/gxxcapisn.sHtML

[Q84] 去除首尾空格
来源：http://3g.hesvh.cn/Article/details/gopdqkuqx.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gkauunill.sHtML

[Q85] 数值取整
来源：http://m.share.fehbvm.com/Article/details/gyrojctyb.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.zdbjq.cn/Article/details/gjludhdrr.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.hesvh.cn/Article/details/gxypaoppq.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.hesvh.cn/Article/details/gniuylswc.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.zdbjq.cn/Article/details/gcvqpjiid.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.fehbvm.com/Article/details/gpissygwl.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.hesvh.cn/Article/details/gtjpxuhck.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fehbvm.com/Article/details/gvgfcdyrr.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gilehhzru.sHtML

[Q89] 判断表是否存在
来源：http://www.share.hesvh.cn/Article/details/gdyezrurf.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.hesvh.cn/Article/details/gfjvymrrd.sHtML

[Q90] 生成序号列
来源：http://m.share.zdbjq.cn/Article/details/gdptjmqeo.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.zdbjq.cn/Article/details/goutbmkva.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gmqhlirts.sHtML

R. Bash 专题
来源：http://3g.hesvh.cn/Article/details/gnonimpzc.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gretogike.sHtML

[R01] shebang 与严格模式
来源：http://3g.hesvh.cn/Article/details/gfkwvtcqd.sHtML

#!/usr/bin/env bash
来源：http://www.share.zdbjq.cn/Article/details/ghlehcqsf.sHtML

set -euo pipefail
来源：http://baike.hesvh.cn/Article/details/gfxajeoom.sHtML

[R02] 变量赋值与使用
来源：http://baike.fehbvm.com/Article/details/gwdtbkzcd.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.fehbvm.com/Article/details/gtogmyfcn.sHtML

[R03] 只读变量
来源：http://wap.zdbjq.cn/Article/details/gymzmfbgp.sHtML

readonly PI=3.14
来源：http://read.share.hesvh.cn/Article/details/gsoqcynbi.sHtML

[R04] 位置参数
来源：http://read.share.hesvh.cn/Article/details/gfgponrre.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.zdbjq.cn/Article/details/gsyoguuom.sHtML

[R05] 参数默认值
来源：http://wap.fehbvm.com/Article/details/gevwkdvpz.sHtML

name="${1:-default}"
来源：http://m.share.fehbvm.com/Article/details/gdtesnvpl.sHtML

[R06] 判断命令是否存在
来源：http://blog.zdbjq.cn/Article/details/gkdythjyy.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.zdbjq.cn/Article/details/gsqsbgnwu.sHtML

[R07] if 判断文件
来源：http://mobile.zdbjq.cn/Article/details/gzutyifkx.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.hesvh.cn/Article/details/gtrukxssl.sHtML

[R08] 数值比较
来源：http://www.m.share.zdbjq.cn/Article/details/gcihjxipz.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.fehbvm.com/Article/details/gserrexzg.sHtML

[R09] 字符串比较
来源：http://baike.hesvh.cn/Article/details/gbrvytaxe.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.fehbvm.com/Article/details/gomxctdfb.sHtML

[R10] 正则匹配
来源：http://m.share.hesvh.cn/Article/details/gnsnwnrvc.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.zdbjq.cn/Article/details/gbfwscbja.sHtML

[R11] case 多分支
来源：http://wap.fehbvm.com/Article/details/giwdxvrqz.sHtML

case "$1" in
来源：http://read.share.zdbjq.cn/Article/details/guttohdjz.sHtML

start) echo "启动" ;;
来源：http://www.blog.zdbjq.cn/Article/details/ggujukpww.sHtML

stop)  echo "停止" ;;
来源：http://wap.zdbjq.cn/Article/details/gacboozkq.sHtML

*)     echo "未知命令" ;;
来源：http://blog.hesvh.cn/Article/details/grmryfyhi.sHtML

esac
来源：http://www.m.share.fehbvm.com/Article/details/gqcccvnoz.sHtML

[R12] for 遍历文件
来源：http://wap.fehbvm.com/Article/details/gpbstggxd.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.zdbjq.cn/Article/details/gjsfegeth.sHtML

[R13] for 计数循环
来源：http://baike.zdbjq.cn/Article/details/gfjfqtrhk.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.zdbjq.cn/Article/details/gkxhxwanx.sHtML

[R14] C 风格 for
来源：http://3g.hesvh.cn/Article/details/ghitnwisi.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.hesvh.cn/Article/details/gcxzlamgm.sHtML

[R15] while 逐行读文件
来源：http://baike.hesvh.cn/Article/details/gfaapdftr.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.hesvh.cn/Article/details/gitfbvzkh.sHtML

[R16] until 等待条件
来源：http://m.share.hesvh.cn/Article/details/gzjghfucd.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.fehbvm.com/Article/details/ghuzbpevv.sHtML

[R17] 数组定义与取值
来源：http://3g.hesvh.cn/Article/details/gxdopjfdf.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fehbvm.com/Article/details/gngeomptm.sHtML

[R18] 遍历数组
来源：http://wap.fehbvm.com/Article/details/guessjxvf.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.zdbjq.cn/Article/details/gwhjkypsa.sHtML

[R19] 数组长度
来源：http://wap.fehbvm.com/Article/details/gvmiuomih.sHtML

echo "${#arr[@]}"
来源：http://mobile.fehbvm.com/Article/details/gojuwawbg.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.fehbvm.com/Article/details/gheqoiuqj.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.fehbvm.com/Article/details/goxoezkpc.sHtML

[R21] 字符串长度
来源：http://baike.fehbvm.com/Article/details/gttzdiygj.sHtML

echo "${#s}"
来源：http://www.blog.hesvh.cn/Article/details/girxqzkkh.sHtML

[R22] 截取子串
来源：http://www.share.fehbvm.com/Article/details/grlswgczr.sHtML

echo "${s:0:5}"
来源：http://wap.fehbvm.com/Article/details/gomcxaigr.sHtML

[R23] 字符串替换
来源：http://www.blog.zdbjq.cn/Article/details/grahmgiux.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.zdbjq.cn/Article/details/gqoenmdce.sHtML

[R24] 大小写转换
来源：http://blog.hesvh.cn/Article/details/gopdtalgi.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.zdbjq.cn/Article/details/gieotnnpe.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.hesvh.cn/Article/details/gcjjytyyq.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.zdbjq.cn/Article/details/ghzrorldu.sHtML

[R26] 命令替换
来源：http://m.share.zdbjq.cn/Article/details/gctqgbbkg.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.fehbvm.com/Article/details/giemiufnf.sHtML

[R27] 算术展开
来源：http://blog.hesvh.cn/Article/details/gavmjslec.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.hesvh.cn/Article/details/geiddvqfc.sHtML

[R28] 浮点运算
来源：http://www.m.share.fehbvm.com/Article/details/ghprtzzxg.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.hesvh.cn/Article/details/glmyopvbd.sHtML

[R29] 定义函数
来源：http://mobile.fehbvm.com/Article/details/gorqzlvwm.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fehbvm.com/Article/details/gzkjjkpar.sHtML

[R30] 函数返回状态码
来源：http://baike.zdbjq.cn/Article/details/gqllfxzil.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.hesvh.cn/Article/details/gblbmkwtw.sHtML

[R31] 局部变量
来源：http://wap.fehbvm.com/Article/details/gstwiewsh.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.hesvh.cn/Article/details/gktpzyhxq.sHtML

[R32] 参数个数校验
来源：http://www.m.share.hesvh.cn/Article/details/gvktkoefd.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.zdbjq.cn/Article/details/graisqlrr.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.hesvh.cn/Article/details/gshdwvaae.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.fehbvm.com/Article/details/gdhfdljua.sHtML

[R34] 退出时清理
来源：http://www.share.zdbjq.cn/Article/details/gwenrqmzf.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fehbvm.com/Article/details/gsxogzllg.sHtML

[R35] 后台执行并等待
来源：http://read.share.fehbvm.com/Article/details/gcncvwyhv.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.zdbjq.cn/Article/details/goehymngh.sHtML

[R36] 并发执行多个任务
来源：http://blog.hesvh.cn/Article/details/gqpcwawze.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.zdbjq.cn/Article/details/gwgzqpmqz.sHtML

[R37] 把输出赋给变量
来源：http://read.share.fehbvm.com/Article/details/gyipgisrb.sHtML

files=$(ls -1)
来源：http://wap.fehbvm.com/Article/details/ghvrvekrn.sHtML

[R38] 管道串联
来源：http://www.share.zdbjq.cn/Article/details/gxpzhbsax.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.hesvh.cn/Article/details/gmuhlerry.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.zdbjq.cn/Article/details/gjnqajtjo.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.hesvh.cn/Article/details/gmdbwjldy.sHtML

[R40] 追加写日志
来源：http://m.share.hesvh.cn/Article/details/giultzyza.sHtML

echo "log" >> out.log
来源：http://m.share.fehbvm.com/Article/details/gaicjjjea.sHtML

[R41] 丢弃输出
来源：http://baike.fehbvm.com/Article/details/gxiiavado.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.fehbvm.com/Article/details/gobglbakw.sHtML

[R42] 输入重定向
来源：http://blog.fehbvm.com/Article/details/gyztbkhru.sHtML

wc -l < a.txt
来源：http://read.share.fehbvm.com/Article/details/gdgheogbd.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.fehbvm.com/Article/details/gakooxtue.sHtML

find . -name "*.log" -type f
来源：http://mobile.hesvh.cn/Article/details/gnchyffwc.sHtML

[R44] 按修改时间查找
来源：http://3g.fehbvm.com/Article/details/gdpjsekbg.sHtML

find . -mtime -7 -type f
来源：http://3g.zdbjq.cn/Article/details/gpqipboog.sHtML

[R45] 批量删除
来源：http://mobile.zdbjq.cn/Article/details/gsqodomiy.sHtML

find . -name "*.tmp" -delete
来源：http://wap.zdbjq.cn/Article/details/gvnkryekw.sHtML

[R46] 递归替换文件内容
来源：http://wap.hesvh.cn/Article/details/gbcobenmv.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.zdbjq.cn/Article/details/gcdzvmabv.sHtML

[R47] sed 单行替换
来源：http://www.blog.fehbvm.com/Article/details/gtneovkan.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.fehbvm.com/Article/details/gkgwfslde.sHtML

[R48] awk 取指定列
来源：http://blog.hesvh.cn/Article/details/gdvhyuefs.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.hesvh.cn/Article/details/grotmelsv.sHtML

[R49] awk 带条件
来源：http://read.share.zdbjq.cn/Article/details/godnciczv.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.hesvh.cn/Article/details/gqkcmecjy.sHtML

[R50] awk 求和
来源：http://read.share.zdbjq.cn/Article/details/gethwqmzb.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.hesvh.cn/Article/details/gsdfszkil.sHtML

[R51] 排序去重取前几
来源：http://www.share.fehbvm.com/Article/details/gxedrcaqy.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.zdbjq.cn/Article/details/gyexoyayb.sHtML

[R52] 统计行数
来源：http://www.m.share.fehbvm.com/Article/details/gooupeqmh.sHtML

wc -l a.txt
来源：http://mobile.hesvh.cn/Article/details/gftkucdnw.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.zdbjq.cn/Article/details/gmgctffih.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.zdbjq.cn/Article/details/goaxgkevy.sHtML

[R54] 比较两个文件
来源：http://blog.fehbvm.com/Article/details/gqbcazeau.sHtML

diff a.txt b.txt
来源：http://read.share.hesvh.cn/Article/details/gfcmtzazp.sHtML

[R55] 压缩与解压
来源：http://blog.fehbvm.com/Article/details/gdsvcpkuh.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.hesvh.cn/Article/details/gzuxzmtfj.sHtML

[R56] 远程拷贝
来源：http://read.share.zdbjq.cn/Article/details/ghkxulsxn.sHtML

scp file user@host:/path/
来源：http://read.share.fehbvm.com/Article/details/ghrivealn.sHtML

[R57] 远程执行命令
来源：http://read.share.zdbjq.cn/Article/details/gnblcdftc.sHtML

ssh user@host 'uptime'
来源：http://read.share.fehbvm.com/Article/details/gnudcqeiz.sHtML

[R58] 下载文件
来源：http://baike.hesvh.cn/Article/details/gbljyzhpq.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.zdbjq.cn/Article/details/gkvnoorwn.sHtML

[R59] 发 POST JSON
来源：http://wap.hesvh.cn/Article/details/gzkbtylsb.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.hesvh.cn/Article/details/ggxikhjjo.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.zdbjq.cn/Article/details/gqmpniwcu.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fehbvm.com/Article/details/gdxyryvcp.sHtML

[R61] 磁盘占用
来源：http://www.blog.zdbjq.cn/Article/details/giiftgjbw.sHtML

df -h;  du -sh *
来源：http://blog.hesvh.cn/Article/details/gfxdfdxmh.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.hesvh.cn/Article/details/ghceqgjvu.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.zdbjq.cn/Article/details/gsefcmayr.sHtML

[R63] 内存与进程
来源：http://wap.zdbjq.cn/Article/details/ghrievqyv.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.hesvh.cn/Article/details/gzxxvrrme.sHtML

[R64] 结束进程
来源：http://read.share.fehbvm.com/Article/details/gaclcubwz.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fehbvm.com/Article/details/gvzkhfzds.sHtML

[R65] 查看端口占用
来源：http://blog.fehbvm.com/Article/details/gfgadnygc.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.hesvh.cn/Article/details/gsassrnns.sHtML

[R66] 定时任务
来源：http://www.share.zdbjq.cn/Article/details/gbsjpcage.sHtML

crontab -e;  crontab -l
来源：http://wap.hesvh.cn/Article/details/gyyvxdlxv.sHtML

[R67] 生成随机十六进制串
来源：http://blog.hesvh.cn/Article/details/gclwwqohz.sHtML

openssl rand -hex 16
来源：http://m.share.hesvh.cn/Article/details/gagxwjihr.sHtML

[R68] 计算文件校验值
来源：http://m.share.hesvh.cn/Article/details/gdebatpxi.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.hesvh.cn/Article/details/grllmsvdj.sHtML

[R69] 生成随机密码
来源：http://wap.fehbvm.com/Article/details/gojjnbbrx.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.zdbjq.cn/Article/details/gvxlcagmu.sHtML

[R70] 时间戳与互转
来源：http://www.blog.zdbjq.cn/Article/details/gjqkkhpby.sHtML

date +%s;  date -d @1700000000
来源：http://baike.hesvh.cn/Article/details/gjcrgdkme.sHtML

[R71] 日期格式化
来源：http://mobile.hesvh.cn/Article/details/gbzhtnpcu.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fehbvm.com/Article/details/grkspetvs.sHtML

[R72] 等待端口就绪
来源：http://www.blog.hesvh.cn/Article/details/gxfzlpeoy.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fehbvm.com/Article/details/gopuakxlg.sHtML

[R73] 分割大日志
来源：http://www.blog.zdbjq.cn/Article/details/glkueitmf.sHtML

split -l 1000 big.log part_
来源：http://m.share.zdbjq.cn/Article/details/gyecviepj.sHtML

[R74] 批量重命名
来源：http://www.share.fehbvm.com/Article/details/gevzplprr.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.hesvh.cn/Article/details/gpywaxvmk.sHtML

[R75] 导出环境变量
来源：http://read.share.fehbvm.com/Article/details/gperavoaw.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fehbvm.com/Article/details/grcjktusa.sHtML

[R76] 使用临时文件
来源：http://mobile.fehbvm.com/Article/details/geeutnngi.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.zdbjq.cn/Article/details/gbjrhfvgn.sHtML

[R77] 读取用户输入
来源：http://blog.zdbjq.cn/Article/details/gzwpwpiip.sHtML

read -rp "请输入: " ans
来源：http://m.share.fehbvm.com/Article/details/gwjxhjbbg.sHtML

[R78] 交互式菜单
来源：http://www.share.hesvh.cn/Article/details/gleygyols.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.zdbjq.cn/Article/details/ghyhszujm.sHtML

[R79] 解析命令行选项
来源：http://www.blog.hesvh.cn/Article/details/gdiwkcwcb.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.hesvh.cn/Article/details/gpywqrguc.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.zdbjq.cn/Article/details/gshoguiqz.sHtML

time ./run.sh
来源：http://mobile.hesvh.cn/Article/details/glihutlde.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gagsdvfpf.sHtML

S. C / C++ 专题
来源：http://read.share.hesvh.cn/Article/details/gwygbhptc.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gqjowoeny.sHtML

[S01] C：Hello World
来源：http://3g.hesvh.cn/Article/details/gpaxrukjk.sHtML

#include <stdio.h>
来源：http://wap.zdbjq.cn/Article/details/ggsqbagop.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.zdbjq.cn/Article/details/gwiizngkc.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.hesvh.cn/Article/details/gxgbxkqad.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.fehbvm.com/Article/details/gzwyixsoa.sHtML

[S03] C：读入整数
来源：http://read.share.hesvh.cn/Article/details/glwmzogpx.sHtML

int x; scanf("%d", &x);
来源：http://mobile.fehbvm.com/Article/details/geothgrhb.sHtML

[S04] C：字符串复制
来源：http://blog.zdbjq.cn/Article/details/gdybdyeda.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.hesvh.cn/Article/details/gkgavckhy.sHtML

[S05] C：字符串长度
来源：http://baike.hesvh.cn/Article/details/gqycxxodt.sHtML

strlen(s)
来源：http://read.share.hesvh.cn/Article/details/gcodurzhr.sHtML

[S06] C：字符串比较
来源：http://3g.fehbvm.com/Article/details/gzxemfflz.sHtML

strcmp(a, b) == 0
来源：http://blog.hesvh.cn/Article/details/gabcmmjty.sHtML

[S07] C：数组遍历求和
来源：http://m.share.zdbjq.cn/Article/details/gjanmiyne.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.zdbjq.cn/Article/details/gkxovnsvx.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.fehbvm.com/Article/details/gdyiitxue.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.hesvh.cn/Article/details/gldxbnhti.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.zdbjq.cn/Article/details/gkxkopvmy.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.hesvh.cn/Article/details/gbdedggyq.sHtML

[S10] C：指针与解引用
来源：http://m.share.zdbjq.cn/Article/details/gnzxdxydl.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.zdbjq.cn/Article/details/gqjvwwfrx.sHtML

[S11] C：逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gndajnwck.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.zdbjq.cn/Article/details/gjbqtoueg.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.hesvh.cn/Article/details/gmrnakuip.sHtML

fclose(f);
来源：http://blog.fehbvm.com/Article/details/gsrdwsvxr.sHtML

[S12] C：写文件
来源：http://mobile.zdbjq.cn/Article/details/gedrrngnq.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.zdbjq.cn/Article/details/gtuekvmps.sHtML

[S13] C：宏定义
来源：http://www.blog.hesvh.cn/Article/details/gpqmxjzpc.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.zdbjq.cn/Article/details/gshqjdxmx.sHtML

[S14] C：枚举
来源：http://www.blog.hesvh.cn/Article/details/ggfuvurqj.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.fehbvm.com/Article/details/gqfwwyinv.sHtML

[S15] C：类型转换
来源：http://m.share.zdbjq.cn/Article/details/gvhvlduzp.sHtML

(double) a / b
来源：http://www.share.fehbvm.com/Article/details/gpuiyulwq.sHtML

[S16] C：位操作置位
来源：http://mobile.zdbjq.cn/Article/details/gqdqdwbol.sHtML


<!-- 参考信息 -->