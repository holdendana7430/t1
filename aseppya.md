代发 wailian999

[Q38] 全外连接（PostgreSQL）
来源：http://wap.hesvh.cn/Article/details/gafwprldh.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.zdbjq.cn/Article/details/ghrfodent.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.zdbjq.cn/Article/details/gboepsnbh.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.fehbvm.com/Article/details/gxsusnphm.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.zdbjq.cn/Article/details/gewuklzsa.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.zdbjq.cn/Article/details/gporvujgr.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.fehbvm.com/Article/details/gytqxddmz.sHtML

[Q41] 多表连接
来源：http://www.share.fehbvm.com/Article/details/gcpdmkeoi.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.fehbvm.com/Article/details/gcoyldgmo.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.hesvh.cn/Article/details/gcrdxpiuf.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.zdbjq.cn/Article/details/gioswxpxo.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.hesvh.cn/Article/details/guvblmvnl.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.zdbjq.cn/Article/details/guslyuyeg.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.hesvh.cn/Article/details/gmbnaravz.sHtML

[Q43] 标量子查询
来源：http://m.share.hesvh.cn/Article/details/gxsqgcsin.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.zdbjq.cn/Article/details/gdiwnzozz.sHtML

[Q44] IN 子查询
来源：http://mobile.fehbvm.com/Article/details/gywvocvup.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.hesvh.cn/Article/details/gkfvnwiyh.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.hesvh.cn/Article/details/ggwuodiaa.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.zdbjq.cn/Article/details/gyjsxdezd.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.zdbjq.cn/Article/details/gvsjcrcxt.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.hesvh.cn/Article/details/ghbbfbrbf.sHtML

[Q47] 与平均值比较
来源：http://blog.hesvh.cn/Article/details/gzghxwbqg.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.hesvh.cn/Article/details/gyshizzso.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.hesvh.cn/Article/details/gztrmcviz.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.hesvh.cn/Article/details/gixindoxs.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.fehbvm.com/Article/details/gywjgrwpc.sHtML

[Q49] 更新单行
来源：http://mobile.hesvh.cn/Article/details/ghrthlyns.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.hesvh.cn/Article/details/gmgeyimsc.sHtML

[Q50] 批量更新
来源：http://m.share.fehbvm.com/Article/details/grlzpknnn.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.zdbjq.cn/Article/details/gyvsygmri.sHtML

[Q51] 用子查询更新
来源：http://3g.zdbjq.cn/Article/details/gikxuqzco.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.fehbvm.com/Article/details/govcztjpy.sHtML

[Q52] 删除指定行
来源：http://www.share.fehbvm.com/Article/details/gfrhawkjn.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.hesvh.cn/Article/details/gzrizcgsg.sHtML

[Q53] 按条件删除
来源：http://read.share.fehbvm.com/Article/details/gdonzhyxo.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.zdbjq.cn/Article/details/gtvnodoal.sHtML

[Q54] 清空表
来源：http://3g.zdbjq.cn/Article/details/gtmvaaegw.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.zdbjq.cn/Article/details/gozgsgzdo.sHtML

[Q55] 排名（并列占位）
来源：http://baike.fehbvm.com/Article/details/gggodwxqw.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.zdbjq.cn/Article/details/gsnlhyekb.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.hesvh.cn/Article/details/gnublnhrf.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.zdbjq.cn/Article/details/gslwsjpfc.sHtML

[Q57] 行号
来源：http://m.share.zdbjq.cn/Article/details/gqoarlfqq.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.zdbjq.cn/Article/details/gagutkuoh.sHtML

[Q58] 累计求和
来源：http://baike.zdbjq.cn/Article/details/gweuplcds.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gfybbrgzm.sHtML

[Q59] 分组内累计
来源：http://read.share.zdbjq.cn/Article/details/gmuzrrsba.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gpfbgevzd.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.hesvh.cn/Article/details/gnrqtluln.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.hesvh.cn/Article/details/gauwbacyn.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gtrxffqzq.sHtML

[Q61] 移动平均
来源：http://mobile.fehbvm.com/Article/details/gmgsntcoc.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.hesvh.cn/Article/details/glnsetjko.sHtML

[Q62] 分组占比
来源：http://m.share.zdbjq.cn/Article/details/gxxywrmsb.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.hesvh.cn/Article/details/gnxzretya.sHtML

[Q63] 开启事务
来源：http://www.blog.fehbvm.com/Article/details/ggycnxfeh.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.zdbjq.cn/Article/details/gsobgpvts.sHtML

[Q64] 提交事务
来源：http://mobile.fehbvm.com/Article/details/gdpgrhhgm.sHtML

COMMIT;
来源：http://www.blog.zdbjq.cn/Article/details/guckxjedp.sHtML

[Q65] 回滚事务
来源：http://www.blog.fehbvm.com/Article/details/gnvvmeiou.sHtML

ROLLBACK;
来源：http://wap.hesvh.cn/Article/details/gumbeszhp.sHtML

[Q66] 行锁查询
来源：http://m.share.zdbjq.cn/Article/details/gmhzirlgf.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.hesvh.cn/Article/details/givszjctw.sHtML

[Q67] 设置隔离级别
来源：http://read.share.fehbvm.com/Article/details/guvqfaghq.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.hesvh.cn/Article/details/gflfybkkh.sHtML

[Q68] 保存点
来源：http://blog.zdbjq.cn/Article/details/gagstalis.sHtML

SAVEPOINT sp1;
来源：http://baike.zdbjq.cn/Article/details/gqauqdsgg.sHtML

ROLLBACK TO sp1;
来源：http://mobile.zdbjq.cn/Article/details/gzjuntisd.sHtML

[Q69] 查看执行计划
来源：http://3g.zdbjq.cn/Article/details/gbhyjvref.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.fehbvm.com/Article/details/gxxrlttgc.sHtML

[Q70] 更新统计信息
来源：http://mobile.fehbvm.com/Article/details/geuyhzvbn.sHtML

ANALYZE TABLE users;
来源：http://mobile.zdbjq.cn/Article/details/gikvlnefa.sHtML

[Q71] 查看建表语句
来源：http://wap.fehbvm.com/Article/details/gpqsdjudh.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.hesvh.cn/Article/details/gmvcvrwmk.sHtML

[Q72] 查看索引
来源：http://www.share.fehbvm.com/Article/details/gpeqnbmlw.sHtML

SHOW INDEX FROM users;
来源：http://wap.zdbjq.cn/Article/details/glfjtgzwu.sHtML

[Q73] 查看表状态
来源：http://blog.hesvh.cn/Article/details/gitfcmhla.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.hesvh.cn/Article/details/gmmqobuyi.sHtML

[Q74] 强制使用索引
来源：http://3g.fehbvm.com/Article/details/gmmphneox.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.fehbvm.com/Article/details/gcmjzehat.sHtML

[Q75] 日期格式化
来源：http://blog.fehbvm.com/Article/details/gauspyqts.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gvikpulzo.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.zdbjq.cn/Article/details/garpazcim.sHtML

[Q76] 按天统计
来源：http://www.blog.fehbvm.com/Article/details/gsnvtnymr.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.zdbjq.cn/Article/details/gcdqyoqzd.sHtML

[Q77] 时间加减
来源：http://read.share.zdbjq.cn/Article/details/gvraoqoyb.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.zdbjq.cn/Article/details/gczgvgmsd.sHtML

[Q78] 当前时间
来源：http://www.m.share.zdbjq.cn/Article/details/ggnklgpcl.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.fehbvm.com/Article/details/gmhrdzxor.sHtML

[Q79] 字符串拼接
来源：http://read.share.zdbjq.cn/Article/details/gtgvtocje.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.zdbjq.cn/Article/details/grcyvshfp.sHtML

[Q80] 字符串截取
来源：http://www.share.zdbjq.cn/Article/details/gobzkuqmz.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gypspztaw.sHtML

[Q81] 字符串替换
来源：http://www.share.fehbvm.com/Article/details/ghjmnzhms.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.hesvh.cn/Article/details/gnzqbqlmj.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.hesvh.cn/Article/details/gvknskhth.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/ggztbucvy.sHtML

[Q83] 大小写转换
来源：http://wap.hesvh.cn/Article/details/gjljbxoyj.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/gunnpfotl.sHtML

[Q84] 去除首尾空格
来源：http://3g.hesvh.cn/Article/details/guksaiexv.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/gcivmoayd.sHtML

[Q85] 数值取整
来源：http://m.share.zdbjq.cn/Article/details/gcedwkdlw.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.fehbvm.com/Article/details/gnaimcznl.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.hesvh.cn/Article/details/ghosabnkc.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.fehbvm.com/Article/details/gjfvagjta.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.hesvh.cn/Article/details/grfcxkgxw.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.zdbjq.cn/Article/details/gmwctslwg.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.fehbvm.com/Article/details/gticmscns.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.hesvh.cn/Article/details/golcdjzco.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.zdbjq.cn/Article/details/glmktkodt.sHtML

[Q89] 判断表是否存在
来源：http://m.share.zdbjq.cn/Article/details/gxxstejzd.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.fehbvm.com/Article/details/gcvuozdsi.sHtML

[Q90] 生成序号列
来源：http://www.m.share.zdbjq.cn/Article/details/gkrumkwmk.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.zdbjq.cn/Article/details/gqbacmhnu.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gtbeuerdc.sHtML

R. Bash 专题
来源：http://blog.fehbvm.com/Article/details/ghtxlupbp.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gjcweluyl.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.hesvh.cn/Article/details/gqlapzisi.sHtML

#!/usr/bin/env bash
来源：http://www.blog.fehbvm.com/Article/details/gsydsfmmh.sHtML

set -euo pipefail
来源：http://www.m.share.fehbvm.com/Article/details/ghtapettg.sHtML

[R02] 变量赋值与使用
来源：http://3g.hesvh.cn/Article/details/gklomfyfl.sHtML

name="Tom"; echo "$name"
来源：http://read.share.fehbvm.com/Article/details/gduamfvsb.sHtML

[R03] 只读变量
来源：http://wap.zdbjq.cn/Article/details/gwuqjygtj.sHtML

readonly PI=3.14
来源：http://www.m.share.fehbvm.com/Article/details/gegcginsn.sHtML

[R04] 位置参数
来源：http://read.share.zdbjq.cn/Article/details/gxufzyixg.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.hesvh.cn/Article/details/givrnbnjg.sHtML

[R05] 参数默认值
来源：http://read.share.fehbvm.com/Article/details/ghdsyxypb.sHtML

name="${1:-default}"
来源：http://www.share.hesvh.cn/Article/details/gfhhkjvjd.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.hesvh.cn/Article/details/gpfzyufwu.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.zdbjq.cn/Article/details/gqmyklxqz.sHtML

[R07] if 判断文件
来源：http://baike.fehbvm.com/Article/details/gekkybesj.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.hesvh.cn/Article/details/gdulccocu.sHtML

[R08] 数值比较
来源：http://www.m.share.fehbvm.com/Article/details/gcyryfxdi.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.hesvh.cn/Article/details/gfdpuklfw.sHtML

[R09] 字符串比较
来源：http://mobile.fehbvm.com/Article/details/gpftqtcaq.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gcppimqdh.sHtML

[R10] 正则匹配
来源：http://mobile.fehbvm.com/Article/details/gsjnoshtg.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.fehbvm.com/Article/details/gfwdchfpa.sHtML

[R11] case 多分支
来源：http://3g.zdbjq.cn/Article/details/gpwkallva.sHtML

case "$1" in
来源：http://baike.zdbjq.cn/Article/details/guctxjtad.sHtML

start) echo "启动" ;;
来源：http://blog.fehbvm.com/Article/details/gkifzraqi.sHtML

stop)  echo "停止" ;;
来源：http://wap.zdbjq.cn/Article/details/gkemcxgue.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.hesvh.cn/Article/details/gvwzfbeek.sHtML

esac
来源：http://www.blog.zdbjq.cn/Article/details/gtfxrcnyk.sHtML

[R12] for 遍历文件
来源：http://baike.zdbjq.cn/Article/details/glrubiuhy.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.fehbvm.com/Article/details/gwmrdhsqw.sHtML

[R13] for 计数循环
来源：http://blog.zdbjq.cn/Article/details/ghzhxvhxt.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.zdbjq.cn/Article/details/gcvtlbrbm.sHtML

[R14] C 风格 for
来源：http://mobile.zdbjq.cn/Article/details/ggpfhdsxh.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.fehbvm.com/Article/details/gyrfhkmou.sHtML

[R15] while 逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gxgrqrmgu.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.fehbvm.com/Article/details/gbmoexhuk.sHtML

[R16] until 等待条件
来源：http://3g.hesvh.cn/Article/details/gfnajnbjd.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.hesvh.cn/Article/details/goaqdvgmx.sHtML

[R17] 数组定义与取值
来源：http://baike.hesvh.cn/Article/details/glzpcraaq.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.fehbvm.com/Article/details/gpsvaiptj.sHtML

[R18] 遍历数组
来源：http://read.share.fehbvm.com/Article/details/gpgdhiqlg.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.zdbjq.cn/Article/details/gryuswiif.sHtML

[R19] 数组长度
来源：http://wap.hesvh.cn/Article/details/gynupntei.sHtML

echo "${#arr[@]}"
来源：http://blog.zdbjq.cn/Article/details/gyrfnmeta.sHtML

[R20] 关联数组（字典）
来源：http://baike.hesvh.cn/Article/details/gyfuwoxwe.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.zdbjq.cn/Article/details/gxxmqlhqd.sHtML

[R21] 字符串长度
来源：http://blog.fehbvm.com/Article/details/gijiolrnw.sHtML

echo "${#s}"
来源：http://www.share.fehbvm.com/Article/details/gozlcvmlb.sHtML

[R22] 截取子串
来源：http://3g.hesvh.cn/Article/details/gvnnfksct.sHtML

echo "${s:0:5}"
来源：http://3g.zdbjq.cn/Article/details/gwvbpymzg.sHtML

[R23] 字符串替换
来源：http://m.share.zdbjq.cn/Article/details/gljkyfxjw.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.hesvh.cn/Article/details/gchialxeh.sHtML

[R24] 大小写转换
来源：http://mobile.zdbjq.cn/Article/details/gedrscqcr.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.hesvh.cn/Article/details/grtzcethd.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.hesvh.cn/Article/details/gaqwsjpkm.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fehbvm.com/Article/details/grugkwbod.sHtML

[R26] 命令替换
来源：http://wap.fehbvm.com/Article/details/gyizxmbro.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.zdbjq.cn/Article/details/geoxsqfgw.sHtML

[R27] 算术展开
来源：http://www.m.share.hesvh.cn/Article/details/gzljbtwfn.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.fehbvm.com/Article/details/gdurfdmun.sHtML

[R28] 浮点运算
来源：http://3g.hesvh.cn/Article/details/geyrjiedi.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.fehbvm.com/Article/details/gypmccnxe.sHtML

[R29] 定义函数
来源：http://read.share.zdbjq.cn/Article/details/gxrixztgu.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.zdbjq.cn/Article/details/gvivqnsfs.sHtML

[R30] 函数返回状态码
来源：http://m.share.zdbjq.cn/Article/details/gumbyrlmh.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.zdbjq.cn/Article/details/ghgdebbec.sHtML

[R31] 局部变量
来源：http://blog.fehbvm.com/Article/details/gnlesuwcb.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.fehbvm.com/Article/details/gkqoorztl.sHtML

[R32] 参数个数校验
来源：http://www.blog.hesvh.cn/Article/details/gmlmwmetr.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.hesvh.cn/Article/details/gsnufemhs.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fehbvm.com/Article/details/gqjtxdrss.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.fehbvm.com/Article/details/gpjrhduod.sHtML

[R34] 退出时清理
来源：http://www.blog.fehbvm.com/Article/details/gdypycpcc.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.hesvh.cn/Article/details/gomtwoaox.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fehbvm.com/Article/details/gwfisoxxw.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.zdbjq.cn/Article/details/gygqturyi.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fehbvm.com/Article/details/gqgxcpeik.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.zdbjq.cn/Article/details/gpyulbsfr.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.hesvh.cn/Article/details/gsxhxvjcq.sHtML

files=$(ls -1)
来源：http://www.share.fehbvm.com/Article/details/goqdaecev.sHtML

[R38] 管道串联
来源：http://3g.fehbvm.com/Article/details/gcxlxwzha.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fehbvm.com/Article/details/gfgvwnfwg.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.fehbvm.com/Article/details/gbaeforgt.sHtML

cmd > out.log 2>&1
来源：http://wap.hesvh.cn/Article/details/goqroogwm.sHtML

[R40] 追加写日志
来源：http://blog.fehbvm.com/Article/details/gzsbcjfzv.sHtML

echo "log" >> out.log
来源：http://baike.fehbvm.com/Article/details/ggbtsrdve.sHtML

[R41] 丢弃输出
来源：http://baike.fehbvm.com/Article/details/ggxwcneyu.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.zdbjq.cn/Article/details/gdegdrikp.sHtML

[R42] 输入重定向
来源：http://3g.hesvh.cn/Article/details/gsysgnnrv.sHtML

wc -l < a.txt
来源：http://baike.fehbvm.com/Article/details/grerxpvdk.sHtML

[R43] 按名字查找文件
来源：http://mobile.fehbvm.com/Article/details/gvwjjdhbf.sHtML

find . -name "*.log" -type f
来源：http://baike.fehbvm.com/Article/details/gxnzgsokw.sHtML

[R44] 按修改时间查找
来源：http://baike.hesvh.cn/Article/details/gefnxnblc.sHtML

find . -mtime -7 -type f
来源：http://baike.zdbjq.cn/Article/details/gbismermq.sHtML

[R45] 批量删除
来源：http://baike.hesvh.cn/Article/details/gxertigpx.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.hesvh.cn/Article/details/genycuyad.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.hesvh.cn/Article/details/gtibjomkq.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.fehbvm.com/Article/details/gjvefwwza.sHtML

[R47] sed 单行替换
来源：http://www.share.fehbvm.com/Article/details/gukhjhtaz.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.hesvh.cn/Article/details/gqcqeethc.sHtML

[R48] awk 取指定列
来源：http://m.share.hesvh.cn/Article/details/gmprxdmgv.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.hesvh.cn/Article/details/gyshzusso.sHtML

[R49] awk 带条件
来源：http://read.share.hesvh.cn/Article/details/gkluzhkef.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.zdbjq.cn/Article/details/gckoigdfu.sHtML

[R50] awk 求和
来源：http://read.share.zdbjq.cn/Article/details/gklgehnex.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.fehbvm.com/Article/details/gqwdzzikj.sHtML

[R51] 排序去重取前几
来源：http://baike.zdbjq.cn/Article/details/gzdtfnoma.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.hesvh.cn/Article/details/gckskpulf.sHtML

[R52] 统计行数
来源：http://m.share.zdbjq.cn/Article/details/gznwmunrb.sHtML

wc -l a.txt
来源：http://blog.fehbvm.com/Article/details/gvtliekul.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fehbvm.com/Article/details/gmnqbonrb.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.hesvh.cn/Article/details/gbtjzsdhl.sHtML

[R54] 比较两个文件
来源：http://3g.hesvh.cn/Article/details/gwnxjzbut.sHtML

diff a.txt b.txt
来源：http://blog.fehbvm.com/Article/details/gmwhrqzxn.sHtML

[R55] 压缩与解压
来源：http://blog.fehbvm.com/Article/details/giprqvzli.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fehbvm.com/Article/details/gugyolqmj.sHtML

[R56] 远程拷贝
来源：http://www.m.share.hesvh.cn/Article/details/gblmrpzhj.sHtML

scp file user@host:/path/
来源：http://www.blog.zdbjq.cn/Article/details/gsdbyduyn.sHtML

[R57] 远程执行命令
来源：http://www.blog.fehbvm.com/Article/details/gxicaionm.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fehbvm.com/Article/details/geoxgyiqi.sHtML

[R58] 下载文件
来源：http://www.share.zdbjq.cn/Article/details/gmqvnjitb.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.zdbjq.cn/Article/details/gsuqzwzlf.sHtML

[R59] 发 POST JSON
来源：http://mobile.hesvh.cn/Article/details/gjgpcrwph.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.zdbjq.cn/Article/details/genrwbohn.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fehbvm.com/Article/details/ghyscesgi.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.hesvh.cn/Article/details/grhvnxhwn.sHtML

[R61] 磁盘占用
来源：http://www.m.share.zdbjq.cn/Article/details/gneopcple.sHtML

df -h;  du -sh *
来源：http://wap.zdbjq.cn/Article/details/gcmvuilpu.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.hesvh.cn/Article/details/ggpjjfomv.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.zdbjq.cn/Article/details/gapcrdrsl.sHtML

[R63] 内存与进程
来源：http://blog.zdbjq.cn/Article/details/gyttnbdry.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.fehbvm.com/Article/details/gjwgwxldo.sHtML

[R64] 结束进程
来源：http://3g.fehbvm.com/Article/details/gjbdjnlde.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.fehbvm.com/Article/details/gxxwxoqfy.sHtML

[R65] 查看端口占用
来源：http://wap.zdbjq.cn/Article/details/gtokrrhby.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.zdbjq.cn/Article/details/gbnkvamci.sHtML

[R66] 定时任务
来源：http://blog.fehbvm.com/Article/details/glozogwpe.sHtML

crontab -e;  crontab -l
来源：http://read.share.hesvh.cn/Article/details/gkypolygg.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.fehbvm.com/Article/details/gzcvpdczp.sHtML

openssl rand -hex 16
来源：http://www.blog.zdbjq.cn/Article/details/grfjfohvq.sHtML

[R68] 计算文件校验值
来源：http://read.share.hesvh.cn/Article/details/ghaeqsqwq.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.hesvh.cn/Article/details/gtzeucydh.sHtML

[R69] 生成随机密码
来源：http://m.share.zdbjq.cn/Article/details/gpdmsvobw.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.hesvh.cn/Article/details/gvltwaejo.sHtML

[R70] 时间戳与互转
来源：http://blog.hesvh.cn/Article/details/goremutwt.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.zdbjq.cn/Article/details/gionzqzwi.sHtML

[R71] 日期格式化
来源：http://wap.hesvh.cn/Article/details/ghhxdjmqf.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.hesvh.cn/Article/details/gozfeezms.sHtML

[R72] 等待端口就绪
来源：http://3g.hesvh.cn/Article/details/gtetgufib.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.zdbjq.cn/Article/details/gobfbxkzk.sHtML

[R73] 分割大日志
来源：http://3g.fehbvm.com/Article/details/gqefmaoai.sHtML

split -l 1000 big.log part_
来源：http://m.share.zdbjq.cn/Article/details/gqnbgxhmw.sHtML

[R74] 批量重命名
来源：http://3g.hesvh.cn/Article/details/gmqwqgzix.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.fehbvm.com/Article/details/giwuagfpz.sHtML

[R75] 导出环境变量
来源：http://blog.fehbvm.com/Article/details/gbrjevqzw.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.hesvh.cn/Article/details/gflzxcevk.sHtML

[R76] 使用临时文件
来源：http://www.m.share.zdbjq.cn/Article/details/gabfjmlht.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.zdbjq.cn/Article/details/grnuykkkn.sHtML

[R77] 读取用户输入
来源：http://mobile.fehbvm.com/Article/details/gsxbujgyp.sHtML

read -rp "请输入: " ans
来源：http://blog.zdbjq.cn/Article/details/gjahtnvcj.sHtML

[R78] 交互式菜单
来源：http://baike.zdbjq.cn/Article/details/gqlnscpnu.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.zdbjq.cn/Article/details/ghvdncjug.sHtML

[R79] 解析命令行选项
来源：http://blog.zdbjq.cn/Article/details/gullcfylx.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fehbvm.com/Article/details/gkwctoevr.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.hesvh.cn/Article/details/gohruonlm.sHtML

time ./run.sh
来源：http://www.share.hesvh.cn/Article/details/gsqxwljcz.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gvgkuyasi.sHtML

S. C / C++ 专题
来源：http://3g.hesvh.cn/Article/details/gzboyggkk.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/ghmrohhiz.sHtML

[S01] C：Hello World
来源：http://read.share.zdbjq.cn/Article/details/ganrypaxd.sHtML

#include <stdio.h>
来源：http://www.blog.zdbjq.cn/Article/details/gkjayozoq.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fehbvm.com/Article/details/gghbcxdyl.sHtML

[S02] C：变量与格式化输出
来源：http://blog.fehbvm.com/Article/details/gmrxmmqsl.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fehbvm.com/Article/details/gltkvzvod.sHtML

[S03] C：读入整数
来源：http://baike.fehbvm.com/Article/details/gsavsrvyx.sHtML

int x; scanf("%d", &x);
来源：http://m.share.hesvh.cn/Article/details/gzpqvbxns.sHtML

[S04] C：字符串复制
来源：http://wap.zdbjq.cn/Article/details/ghnkxynsc.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.zdbjq.cn/Article/details/gvqyiqjlh.sHtML

[S05] C：字符串长度
来源：http://www.blog.zdbjq.cn/Article/details/gpqiqhqwr.sHtML

strlen(s)
来源：http://read.share.zdbjq.cn/Article/details/gjyzvekys.sHtML

[S06] C：字符串比较
来源：http://baike.hesvh.cn/Article/details/gjsalfzqs.sHtML

strcmp(a, b) == 0
来源：http://blog.zdbjq.cn/Article/details/ggkhjxoyy.sHtML

[S07] C：数组遍历求和
来源：http://mobile.zdbjq.cn/Article/details/guruttuye.sHtML


<!-- 参考信息 -->