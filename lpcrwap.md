代发 wailian999

[Q36] 左连接
来源：http://www.share.zdbjq.cn/Article/details/gxhgqkftk.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fehbvm.com/Article/details/gjbfugqnm.sHtML

[Q37] 右连接
来源：http://mobile.fehbvm.com/Article/details/gdtmbldlq.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.zdbjq.cn/Article/details/giwzkvmjp.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.fehbvm.com/Article/details/gofkthpsb.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.zdbjq.cn/Article/details/gzvmxeksq.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.hesvh.cn/Article/details/gvlvipwrd.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.fehbvm.com/Article/details/gqclskamz.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.hesvh.cn/Article/details/gazvgnojz.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.zdbjq.cn/Article/details/gllbgirbd.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.zdbjq.cn/Article/details/gzotoztli.sHtML

[Q41] 多表连接
来源：http://wap.zdbjq.cn/Article/details/ghryoebwb.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.fehbvm.com/Article/details/gaynulqzw.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.hesvh.cn/Article/details/gqgwbhtll.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.hesvh.cn/Article/details/gpmozjdoo.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.hesvh.cn/Article/details/gwffcaave.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.hesvh.cn/Article/details/gzhtmhyte.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.fehbvm.com/Article/details/gowgammhj.sHtML

[Q43] 标量子查询
来源：http://m.share.zdbjq.cn/Article/details/ggjpodpux.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.fehbvm.com/Article/details/gouzhydhr.sHtML

[Q44] IN 子查询
来源：http://blog.zdbjq.cn/Article/details/gswngzeix.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.hesvh.cn/Article/details/gjunfgoaq.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.zdbjq.cn/Article/details/gcykwmgzv.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.zdbjq.cn/Article/details/gnbekfwbv.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.hesvh.cn/Article/details/gkwjqobbb.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.hesvh.cn/Article/details/girmreamd.sHtML

[Q47] 与平均值比较
来源：http://www.blog.zdbjq.cn/Article/details/gdzcdcsnj.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.zdbjq.cn/Article/details/gqlbvrzje.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.fehbvm.com/Article/details/grntqspvg.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.zdbjq.cn/Article/details/gajsygxlq.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.hesvh.cn/Article/details/gdovmgyuv.sHtML

[Q49] 更新单行
来源：http://m.share.hesvh.cn/Article/details/gtaftdcee.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.zdbjq.cn/Article/details/gawoyhmch.sHtML

[Q50] 批量更新
来源：http://baike.fehbvm.com/Article/details/gjjfysvsm.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.fehbvm.com/Article/details/gthnjtbew.sHtML

[Q51] 用子查询更新
来源：http://baike.zdbjq.cn/Article/details/gzyeqbeqf.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gfbjqipko.sHtML

[Q52] 删除指定行
来源：http://wap.fehbvm.com/Article/details/gewsixtxl.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.fehbvm.com/Article/details/gqyjhkrqt.sHtML

[Q53] 按条件删除
来源：http://mobile.fehbvm.com/Article/details/grnpceivl.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.hesvh.cn/Article/details/gdzjwjuca.sHtML

[Q54] 清空表
来源：http://blog.fehbvm.com/Article/details/grbjxvmho.sHtML

TRUNCATE TABLE logs;
来源：http://wap.fehbvm.com/Article/details/gkhrkarpw.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.fehbvm.com/Article/details/gcfmhqkpd.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.fehbvm.com/Article/details/gqirfpsxy.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.fehbvm.com/Article/details/giyuwjirf.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.hesvh.cn/Article/details/gcburquch.sHtML

[Q57] 行号
来源：http://read.share.hesvh.cn/Article/details/gbpgoelfv.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.fehbvm.com/Article/details/gsoyzmxdw.sHtML

[Q58] 累计求和
来源：http://www.m.share.zdbjq.cn/Article/details/gsqgnizki.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gydtcpkea.sHtML

[Q59] 分组内累计
来源：http://blog.zdbjq.cn/Article/details/gqruqbacd.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gkizcbfmw.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.fehbvm.com/Article/details/gttiboclo.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.fehbvm.com/Article/details/gchkguelh.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.hesvh.cn/Article/details/grwbfzypz.sHtML

[Q61] 移动平均
来源：http://www.blog.hesvh.cn/Article/details/geybiscqf.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gzvxplthi.sHtML

[Q62] 分组占比
来源：http://3g.hesvh.cn/Article/details/gifsrgxlm.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.zdbjq.cn/Article/details/gozlbrtfa.sHtML

[Q63] 开启事务
来源：http://wap.fehbvm.com/Article/details/gjmlbkrjy.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.fehbvm.com/Article/details/gmyytdohe.sHtML

[Q64] 提交事务
来源：http://baike.zdbjq.cn/Article/details/gxkrmgzzk.sHtML

COMMIT;
来源：http://www.m.share.zdbjq.cn/Article/details/gnynwxlhe.sHtML

[Q65] 回滚事务
来源：http://www.blog.zdbjq.cn/Article/details/gcyukcpmq.sHtML

ROLLBACK;
来源：http://www.m.share.fehbvm.com/Article/details/gifayxvao.sHtML

[Q66] 行锁查询
来源：http://wap.hesvh.cn/Article/details/gttqlcoen.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.fehbvm.com/Article/details/gkoadkgdg.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.hesvh.cn/Article/details/gbixdkbrw.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.zdbjq.cn/Article/details/giaciztip.sHtML

[Q68] 保存点
来源：http://m.share.fehbvm.com/Article/details/gtwqcgkiv.sHtML

SAVEPOINT sp1;
来源：http://read.share.fehbvm.com/Article/details/gubatfywy.sHtML

ROLLBACK TO sp1;
来源：http://www.share.zdbjq.cn/Article/details/gychclfcn.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.hesvh.cn/Article/details/gnzhwzaro.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.zdbjq.cn/Article/details/gvfpuvqgx.sHtML

[Q70] 更新统计信息
来源：http://3g.hesvh.cn/Article/details/gkbzsqevd.sHtML

ANALYZE TABLE users;
来源：http://wap.fehbvm.com/Article/details/gakzhzgba.sHtML

[Q71] 查看建表语句
来源：http://m.share.fehbvm.com/Article/details/gqexuvjmu.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.fehbvm.com/Article/details/gpsxaeifz.sHtML

[Q72] 查看索引
来源：http://www.share.fehbvm.com/Article/details/gkwszubnk.sHtML

SHOW INDEX FROM users;
来源：http://blog.fehbvm.com/Article/details/glgpokkkg.sHtML

[Q73] 查看表状态
来源：http://www.share.zdbjq.cn/Article/details/gzxptumkl.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.zdbjq.cn/Article/details/gbebdyuue.sHtML

[Q74] 强制使用索引
来源：http://www.share.fehbvm.com/Article/details/gtgzpyrma.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.zdbjq.cn/Article/details/gxthrekiq.sHtML

[Q75] 日期格式化
来源：http://baike.fehbvm.com/Article/details/gwynskwyz.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.fehbvm.com/Article/details/gpnjulyav.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.hesvh.cn/Article/details/geztvyctb.sHtML

[Q76] 按天统计
来源：http://read.share.fehbvm.com/Article/details/gwtesudbl.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.zdbjq.cn/Article/details/gbqkphflh.sHtML

[Q77] 时间加减
来源：http://wap.zdbjq.cn/Article/details/gasyqrkua.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.hesvh.cn/Article/details/gjmuflehl.sHtML

[Q78] 当前时间
来源：http://3g.fehbvm.com/Article/details/gnnczovlh.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.hesvh.cn/Article/details/gbhjfrcya.sHtML

[Q79] 字符串拼接
来源：http://mobile.fehbvm.com/Article/details/gxnubdxvq.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.hesvh.cn/Article/details/giuwewgsl.sHtML

[Q80] 字符串截取
来源：http://blog.fehbvm.com/Article/details/gdpsalahl.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gwfqmulfq.sHtML

[Q81] 字符串替换
来源：http://www.blog.hesvh.cn/Article/details/gzpghbror.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.fehbvm.com/Article/details/geckmcoxc.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.zdbjq.cn/Article/details/gvsaelwgz.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/giklakwra.sHtML

[Q83] 大小写转换
来源：http://www.share.hesvh.cn/Article/details/gsplrvjpo.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gfprbgttd.sHtML

[Q84] 去除首尾空格
来源：http://blog.hesvh.cn/Article/details/gqdnmwmom.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gvlwglnvj.sHtML

[Q85] 数值取整
来源：http://blog.fehbvm.com/Article/details/gzvvfmvth.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.hesvh.cn/Article/details/ghryvqbwk.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.hesvh.cn/Article/details/gxezwgfqy.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.fehbvm.com/Article/details/gaxyepghu.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.zdbjq.cn/Article/details/gpwgzopxy.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.hesvh.cn/Article/details/grpwvhywi.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.fehbvm.com/Article/details/gvbralnvf.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.hesvh.cn/Article/details/ggtbpfysm.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.fehbvm.com/Article/details/gfxnzdgtj.sHtML

[Q89] 判断表是否存在
来源：http://read.share.zdbjq.cn/Article/details/gcmeubbss.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.fehbvm.com/Article/details/ghgahxszj.sHtML

[Q90] 生成序号列
来源：http://mobile.hesvh.cn/Article/details/gzwrfhrgw.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.hesvh.cn/Article/details/gxbhdyxnm.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gsjgolmqr.sHtML

R. Bash 专题
来源：http://www.blog.zdbjq.cn/Article/details/gsxyhgxik.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/ghhihnwdi.sHtML

[R01] shebang 与严格模式
来源：http://wap.hesvh.cn/Article/details/gpytchiop.sHtML

#!/usr/bin/env bash
来源：http://mobile.hesvh.cn/Article/details/gajhpfpdb.sHtML

set -euo pipefail
来源：http://read.share.hesvh.cn/Article/details/gtiapbqkz.sHtML

[R02] 变量赋值与使用
来源：http://mobile.zdbjq.cn/Article/details/gdixbmlff.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.zdbjq.cn/Article/details/gdtxwguzf.sHtML

[R03] 只读变量
来源：http://3g.hesvh.cn/Article/details/gjyaieqji.sHtML

readonly PI=3.14
来源：http://read.share.zdbjq.cn/Article/details/gnyikuwdh.sHtML

[R04] 位置参数
来源：http://wap.zdbjq.cn/Article/details/gmsbkeubh.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.fehbvm.com/Article/details/gsbfbrzsp.sHtML

[R05] 参数默认值
来源：http://www.share.zdbjq.cn/Article/details/gccxdcxsq.sHtML

name="${1:-default}"
来源：http://m.share.hesvh.cn/Article/details/grmkekuou.sHtML

[R06] 判断命令是否存在
来源：http://baike.zdbjq.cn/Article/details/grsigymua.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.hesvh.cn/Article/details/gtyvdlgqu.sHtML

[R07] if 判断文件
来源：http://www.share.hesvh.cn/Article/details/gxcmedhhy.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.hesvh.cn/Article/details/gaxfikszi.sHtML

[R08] 数值比较
来源：http://read.share.fehbvm.com/Article/details/ggeumsffg.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.zdbjq.cn/Article/details/gjjluwafz.sHtML

[R09] 字符串比较
来源：http://m.share.fehbvm.com/Article/details/ghdhwzhns.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.hesvh.cn/Article/details/gbaewucmf.sHtML

[R10] 正则匹配
来源：http://www.blog.zdbjq.cn/Article/details/gkzrvygbl.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.hesvh.cn/Article/details/gawnrhsdm.sHtML

[R11] case 多分支
来源：http://www.m.share.hesvh.cn/Article/details/gjpfccwng.sHtML

case "$1" in
来源：http://read.share.hesvh.cn/Article/details/gnbzoggaq.sHtML

start) echo "启动" ;;
来源：http://www.blog.zdbjq.cn/Article/details/gfvtntmws.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.hesvh.cn/Article/details/gyyxywwad.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.fehbvm.com/Article/details/gjpblzayc.sHtML

esac
来源：http://www.m.share.fehbvm.com/Article/details/grwcamrig.sHtML

[R12] for 遍历文件
来源：http://blog.fehbvm.com/Article/details/gnukvcvhu.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.fehbvm.com/Article/details/gbtpwtzhg.sHtML

[R13] for 计数循环
来源：http://read.share.fehbvm.com/Article/details/gwtbyudkm.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.fehbvm.com/Article/details/gtpahcvgn.sHtML

[R14] C 风格 for
来源：http://www.m.share.fehbvm.com/Article/details/ghstwrrho.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.fehbvm.com/Article/details/ggikwfqzc.sHtML

[R15] while 逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/grxqyawmn.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.hesvh.cn/Article/details/guotdtmwa.sHtML

[R16] until 等待条件
来源：http://blog.fehbvm.com/Article/details/gcajpdguo.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.zdbjq.cn/Article/details/gahwkxvnw.sHtML

[R17] 数组定义与取值
来源：http://m.share.fehbvm.com/Article/details/gzyuaxlcm.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.zdbjq.cn/Article/details/gormgtfzi.sHtML

[R18] 遍历数组
来源：http://mobile.hesvh.cn/Article/details/gejckdvhp.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.hesvh.cn/Article/details/gkjtcyskv.sHtML

[R19] 数组长度
来源：http://baike.zdbjq.cn/Article/details/gvqjmaiph.sHtML

echo "${#arr[@]}"
来源：http://wap.hesvh.cn/Article/details/gthtcrycu.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.zdbjq.cn/Article/details/godpjzzwz.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.hesvh.cn/Article/details/gwqqcmssy.sHtML

[R21] 字符串长度
来源：http://baike.fehbvm.com/Article/details/gyshgrrxf.sHtML

echo "${#s}"
来源：http://blog.hesvh.cn/Article/details/gmnjdgwpu.sHtML

[R22] 截取子串
来源：http://blog.hesvh.cn/Article/details/golzkcgkf.sHtML

echo "${s:0:5}"
来源：http://www.m.share.zdbjq.cn/Article/details/guwnzxbeg.sHtML

[R23] 字符串替换
来源：http://www.m.share.hesvh.cn/Article/details/gupzmlwzp.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.hesvh.cn/Article/details/gcofobuip.sHtML

[R24] 大小写转换
来源：http://mobile.hesvh.cn/Article/details/gbjuikstk.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.hesvh.cn/Article/details/gaihfdbyy.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fehbvm.com/Article/details/gexixillc.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.zdbjq.cn/Article/details/gioaeoicm.sHtML

[R26] 命令替换
来源：http://blog.zdbjq.cn/Article/details/gcbbdhvns.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.hesvh.cn/Article/details/gqbbqdhcc.sHtML

[R27] 算术展开
来源：http://3g.fehbvm.com/Article/details/gpujqruux.sHtML

echo $((1 + 2 * 3))
来源：http://baike.zdbjq.cn/Article/details/glnxmbilm.sHtML

[R28] 浮点运算
来源：http://wap.zdbjq.cn/Article/details/gutssyqut.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.hesvh.cn/Article/details/gobaxiiio.sHtML

[R29] 定义函数
来源：http://m.share.hesvh.cn/Article/details/gmvgvsjzu.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.zdbjq.cn/Article/details/gzvtamnen.sHtML

[R30] 函数返回状态码
来源：http://m.share.zdbjq.cn/Article/details/gvetjyzqg.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.fehbvm.com/Article/details/gvvinnvum.sHtML

[R31] 局部变量
来源：http://www.share.zdbjq.cn/Article/details/gexlnokxv.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.zdbjq.cn/Article/details/gnoarkxur.sHtML

[R32] 参数个数校验
来源：http://www.share.zdbjq.cn/Article/details/gwtslbbce.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.zdbjq.cn/Article/details/gnyxivbgr.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.zdbjq.cn/Article/details/gkduwnsis.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.hesvh.cn/Article/details/girwqmbnk.sHtML

[R34] 退出时清理
来源：http://3g.zdbjq.cn/Article/details/gzxmcbrvr.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.hesvh.cn/Article/details/gqbkadlgh.sHtML

[R35] 后台执行并等待
来源：http://blog.zdbjq.cn/Article/details/geuusqdhj.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.hesvh.cn/Article/details/gbdakzwso.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.hesvh.cn/Article/details/gtdmpmphn.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.hesvh.cn/Article/details/grghbtnca.sHtML

[R37] 把输出赋给变量
来源：http://m.share.hesvh.cn/Article/details/ggkbrdtby.sHtML

files=$(ls -1)
来源：http://3g.zdbjq.cn/Article/details/gptgrutqw.sHtML

[R38] 管道串联
来源：http://m.share.zdbjq.cn/Article/details/gdregidsl.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.zdbjq.cn/Article/details/gupxkjuft.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.zdbjq.cn/Article/details/gollcdalj.sHtML

cmd > out.log 2>&1
来源：http://3g.fehbvm.com/Article/details/gsthnhfdd.sHtML

[R40] 追加写日志
来源：http://read.share.zdbjq.cn/Article/details/gttghcorx.sHtML

echo "log" >> out.log
来源：http://baike.fehbvm.com/Article/details/gksfflxww.sHtML

[R41] 丢弃输出
来源：http://3g.zdbjq.cn/Article/details/gjqjayjzo.sHtML

cmd >/dev/null 2>&1
来源：http://blog.hesvh.cn/Article/details/gqcdixcya.sHtML

[R42] 输入重定向
来源：http://www.blog.zdbjq.cn/Article/details/gwkostiaw.sHtML

wc -l < a.txt
来源：http://www.blog.hesvh.cn/Article/details/gouufzdxx.sHtML

[R43] 按名字查找文件
来源：http://read.share.hesvh.cn/Article/details/gpbjwfbjw.sHtML

find . -name "*.log" -type f
来源：http://read.share.zdbjq.cn/Article/details/ggkwzdrka.sHtML

[R44] 按修改时间查找
来源：http://blog.hesvh.cn/Article/details/gfekcchnf.sHtML

find . -mtime -7 -type f
来源：http://read.share.hesvh.cn/Article/details/gnumfolgf.sHtML

[R45] 批量删除
来源：http://mobile.fehbvm.com/Article/details/grqxdorpg.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.hesvh.cn/Article/details/gczbtfbjv.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.zdbjq.cn/Article/details/gsppgnklo.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.fehbvm.com/Article/details/gsmxcubtp.sHtML

[R47] sed 单行替换
来源：http://m.share.fehbvm.com/Article/details/gxhdknzhb.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.hesvh.cn/Article/details/gzbtximsl.sHtML

[R48] awk 取指定列
来源：http://baike.zdbjq.cn/Article/details/gurikmxtw.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.zdbjq.cn/Article/details/ggbkswukl.sHtML

[R49] awk 带条件
来源：http://www.share.fehbvm.com/Article/details/gpgeodxgk.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.zdbjq.cn/Article/details/gsiwbnbcy.sHtML

[R50] awk 求和
来源：http://baike.hesvh.cn/Article/details/gkfoocnij.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.hesvh.cn/Article/details/gzsupdgpy.sHtML

[R51] 排序去重取前几
来源：http://wap.zdbjq.cn/Article/details/gyrjncorj.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.hesvh.cn/Article/details/gujzvhiuj.sHtML

[R52] 统计行数
来源：http://read.share.fehbvm.com/Article/details/gsxjuyvsx.sHtML

wc -l a.txt
来源：http://read.share.hesvh.cn/Article/details/gfttglawb.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.hesvh.cn/Article/details/gszixadrn.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.hesvh.cn/Article/details/gyjqahqsn.sHtML

[R54] 比较两个文件
来源：http://www.blog.zdbjq.cn/Article/details/gqwcqbrpr.sHtML

diff a.txt b.txt
来源：http://blog.zdbjq.cn/Article/details/gdozdnuzs.sHtML

[R55] 压缩与解压
来源：http://read.share.hesvh.cn/Article/details/ggfifupwf.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fehbvm.com/Article/details/ggfcxiuma.sHtML

[R56] 远程拷贝
来源：http://www.share.fehbvm.com/Article/details/gsdbrgbne.sHtML

scp file user@host:/path/
来源：http://blog.zdbjq.cn/Article/details/ghbqcxnmp.sHtML

[R57] 远程执行命令
来源：http://www.share.zdbjq.cn/Article/details/gcnuoaeqc.sHtML

ssh user@host 'uptime'
来源：http://mobile.fehbvm.com/Article/details/gxkpgehoh.sHtML

[R58] 下载文件
来源：http://read.share.hesvh.cn/Article/details/gtsntxhhz.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.zdbjq.cn/Article/details/ghgphvnxx.sHtML

[R59] 发 POST JSON
来源：http://baike.fehbvm.com/Article/details/gmecvnlzz.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.hesvh.cn/Article/details/ghvbnvoof.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fehbvm.com/Article/details/gelwokitl.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.hesvh.cn/Article/details/gehglmvsl.sHtML

[R61] 磁盘占用
来源：http://www.share.hesvh.cn/Article/details/gqxvnravt.sHtML

df -h;  du -sh *
来源：http://wap.hesvh.cn/Article/details/glwlahsyu.sHtML

[R62] 找最占空间的文件
来源：http://wap.hesvh.cn/Article/details/ggsfptbra.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.hesvh.cn/Article/details/gljmjtbwt.sHtML

[R63] 内存与进程
来源：http://blog.zdbjq.cn/Article/details/gqruzbfai.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.zdbjq.cn/Article/details/gqpplkowf.sHtML

[R64] 结束进程
来源：http://mobile.zdbjq.cn/Article/details/gwnflmddz.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fehbvm.com/Article/details/gjsnemmew.sHtML

[R65] 查看端口占用
来源：http://mobile.hesvh.cn/Article/details/gwdfruvjx.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fehbvm.com/Article/details/gyerwoovu.sHtML

[R66] 定时任务
来源：http://mobile.zdbjq.cn/Article/details/gvhormvkq.sHtML

crontab -e;  crontab -l
来源：http://baike.fehbvm.com/Article/details/giozltvss.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.hesvh.cn/Article/details/gzzetpivp.sHtML

openssl rand -hex 16
来源：http://blog.hesvh.cn/Article/details/gtgpdfagc.sHtML

[R68] 计算文件校验值
来源：http://3g.zdbjq.cn/Article/details/glnqiruqu.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gcrtmcido.sHtML

[R69] 生成随机密码
来源：http://read.share.zdbjq.cn/Article/details/gkowbmksr.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.hesvh.cn/Article/details/gvpiqpggv.sHtML

[R70] 时间戳与互转
来源：http://baike.hesvh.cn/Article/details/gtfohjrel.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.zdbjq.cn/Article/details/gzhjmikwk.sHtML

[R71] 日期格式化
来源：http://m.share.fehbvm.com/Article/details/gzzjjfpwq.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.zdbjq.cn/Article/details/gwwmvqkju.sHtML

[R72] 等待端口就绪
来源：http://www.share.fehbvm.com/Article/details/gmvkpyqcs.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.hesvh.cn/Article/details/gtddjdvtz.sHtML

[R73] 分割大日志
来源：http://wap.zdbjq.cn/Article/details/gzibamztr.sHtML

split -l 1000 big.log part_
来源：http://www.blog.hesvh.cn/Article/details/gwgbxmdzo.sHtML

[R74] 批量重命名
来源：http://3g.fehbvm.com/Article/details/ghgzkotsp.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fehbvm.com/Article/details/gvpmjncwq.sHtML

[R75] 导出环境变量
来源：http://www.m.share.fehbvm.com/Article/details/gdlteccua.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.fehbvm.com/Article/details/gaachtbaw.sHtML

[R76] 使用临时文件
来源：http://www.share.hesvh.cn/Article/details/gesatpltp.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.hesvh.cn/Article/details/guaujaspo.sHtML

[R77] 读取用户输入
来源：http://mobile.fehbvm.com/Article/details/ghhpqdfgy.sHtML

read -rp "请输入: " ans
来源：http://read.share.hesvh.cn/Article/details/gqgqlfioc.sHtML

[R78] 交互式菜单
来源：http://www.blog.zdbjq.cn/Article/details/gymcdaopr.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.hesvh.cn/Article/details/gwlezvkmg.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.hesvh.cn/Article/details/gpbesltee.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.fehbvm.com/Article/details/gzbadlhff.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.fehbvm.com/Article/details/gzygnrlqe.sHtML

time ./run.sh
来源：http://baike.hesvh.cn/Article/details/gdmhlhuhb.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gggxpbpiq.sHtML

S. C / C++ 专题
来源：http://www.m.share.hesvh.cn/Article/details/gigfudcpy.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gktluxkax.sHtML

[S01] C：Hello World
来源：http://baike.zdbjq.cn/Article/details/gsoanapwm.sHtML

#include <stdio.h>
来源：http://m.share.zdbjq.cn/Article/details/goxlzpbbq.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.fehbvm.com/Article/details/grjcipewo.sHtML

[S02] C：变量与格式化输出
来源：http://blog.hesvh.cn/Article/details/gmarxtqfy.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.hesvh.cn/Article/details/gawaczmjn.sHtML

[S03] C：读入整数
来源：http://wap.zdbjq.cn/Article/details/gihughadq.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.zdbjq.cn/Article/details/gfxatdcni.sHtML

[S04] C：字符串复制
来源：http://blog.zdbjq.cn/Article/details/gprrvzrul.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.zdbjq.cn/Article/details/gxbgpoyjn.sHtML

[S05] C：字符串长度
来源：http://read.share.fehbvm.com/Article/details/gdrohthha.sHtML


<!-- 参考信息 -->