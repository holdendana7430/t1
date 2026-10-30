代发 wailian999

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.fanxiaobao.xyz/Article/details/geflpockr.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.fanxiaobao.xyz/Article/details/gbrjzryiu.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gehjdlxfg.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/gqpicrlfy.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.fanxiaobao.xyz/Article/details/gjqfnrwxl.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.fanxiaobao.xyz/Article/details/gncfxajfd.sHtML

[Q43] 标量子查询
来源：http://3g.fanxiaobao.xyz/Article/details/gtmezgwmb.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.fanxiaobao.xyz/Article/details/gfisdrhbv.sHtML

[Q44] IN 子查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gygjicbsv.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.fanxiaobao.xyz/Article/details/glyxqzyuz.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.fanxiaobao.xyz/Article/details/gfmzuihhg.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggiamkydt.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gdadjwtky.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggflbtncw.sHtML

[Q47] 与平均值比较
来源：http://wap.fanxiaobao.xyz/Article/details/gqjlbufzc.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.fanxiaobao.xyz/Article/details/goakcjyfo.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/gupttosre.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.fanxiaobao.xyz/Article/details/gipkrhpwj.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnfewkjcf.sHtML

[Q49] 更新单行
来源：http://www.blog.fanxiaobao.xyz/Article/details/glooeojhu.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/gxqiqpeib.sHtML

[Q50] 批量更新
来源：http://m.share.fanxiaobao.xyz/Article/details/gpdphcffa.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.fanxiaobao.xyz/Article/details/gveeiwein.sHtML

[Q51] 用子查询更新
来源：http://read.share.fanxiaobao.xyz/Article/details/gpnzrwgza.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxenllgrs.sHtML

[Q52] 删除指定行
来源：http://m.share.fanxiaobao.xyz/Article/details/gwkmavvnk.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/gqjlwrlgg.sHtML

[Q53] 按条件删除
来源：http://blog.fanxiaobao.xyz/Article/details/gwigbzkav.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.fanxiaobao.xyz/Article/details/gensnhihv.sHtML

[Q54] 清空表
来源：http://3g.fanxiaobao.xyz/Article/details/gvaadckbf.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.fanxiaobao.xyz/Article/details/gafyydowl.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.fanxiaobao.xyz/Article/details/ggzzsckwx.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.fanxiaobao.xyz/Article/details/glsgvqegb.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.fanxiaobao.xyz/Article/details/gwcapeqni.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.fanxiaobao.xyz/Article/details/gprcboult.sHtML

[Q57] 行号
来源：http://m.share.fanxiaobao.xyz/Article/details/girskruev.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gqygcaoop.sHtML

[Q58] 累计求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gsprvzjjr.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmkyybada.sHtML

[Q59] 分组内累计
来源：http://blog.fanxiaobao.xyz/Article/details/gtpiqbwhv.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/glxxvgxsm.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.fanxiaobao.xyz/Article/details/gcexrrltv.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.fanxiaobao.xyz/Article/details/gzbqywsdr.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gknyyxonh.sHtML

[Q61] 移动平均
来源：http://m.share.fanxiaobao.xyz/Article/details/gisqrxeap.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqvxkopjn.sHtML

[Q62] 分组占比
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggcxlwqtj.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.fanxiaobao.xyz/Article/details/gsctlmdpn.sHtML

[Q63] 开启事务
来源：http://blog.fanxiaobao.xyz/Article/details/ghspplfsi.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.fanxiaobao.xyz/Article/details/gzzfkgtzk.sHtML

[Q64] 提交事务
来源：http://wap.fanxiaobao.xyz/Article/details/gggunspmk.sHtML

COMMIT;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghqeokgef.sHtML

[Q65] 回滚事务
来源：http://3g.fanxiaobao.xyz/Article/details/gqfavqinu.sHtML

ROLLBACK;
来源：http://read.share.fanxiaobao.xyz/Article/details/gcyygfucn.sHtML

[Q66] 行锁查询
来源：http://mobile.fanxiaobao.xyz/Article/details/gnrrwpqbf.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.fanxiaobao.xyz/Article/details/gsklrgynk.sHtML

[Q67] 设置隔离级别
来源：http://mobile.fanxiaobao.xyz/Article/details/grxmzwwjj.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.fanxiaobao.xyz/Article/details/gxjmvgjme.sHtML

[Q68] 保存点
来源：http://mobile.fanxiaobao.xyz/Article/details/guisruovp.sHtML

SAVEPOINT sp1;
来源：http://3g.fanxiaobao.xyz/Article/details/gzkpwelzp.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/grhvtfhkl.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gptvimhrw.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.fanxiaobao.xyz/Article/details/gfnbpgrih.sHtML

[Q70] 更新统计信息
来源：http://www.share.fanxiaobao.xyz/Article/details/gznkihunq.sHtML

ANALYZE TABLE users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gdedictug.sHtML

[Q71] 查看建表语句
来源：http://mobile.fanxiaobao.xyz/Article/details/grbeymhhr.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.fanxiaobao.xyz/Article/details/gdpagxmyi.sHtML

[Q72] 查看索引
来源：http://baike.fanxiaobao.xyz/Article/details/gyrllovch.sHtML

SHOW INDEX FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gvyvhkyxl.sHtML

[Q73] 查看表状态
来源：http://wap.fanxiaobao.xyz/Article/details/gktectdwc.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.fanxiaobao.xyz/Article/details/gqdnxprca.sHtML

[Q74] 强制使用索引
来源：http://www.share.fanxiaobao.xyz/Article/details/gossuckas.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzmqnkuyf.sHtML

[Q75] 日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/genyjouvx.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gqgszuuij.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkxvbaelf.sHtML

[Q76] 按天统计
来源：http://wap.fanxiaobao.xyz/Article/details/gbcjftstu.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfwuicwnm.sHtML

[Q77] 时间加减
来源：http://blog.fanxiaobao.xyz/Article/details/gavosbtwo.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjiamkpci.sHtML

[Q78] 当前时间
来源：http://www.blog.fanxiaobao.xyz/Article/details/guqtvppnq.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnsmmryua.sHtML

[Q79] 字符串拼接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gquvkokyv.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzygqcrxq.sHtML

[Q80] 字符串截取
来源：http://baike.fanxiaobao.xyz/Article/details/gjzipycqr.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/ghljraubi.sHtML

[Q81] 字符串替换
来源：http://3g.fanxiaobao.xyz/Article/details/gxiywcpha.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gqghjfwtf.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gspyhneel.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gbrvwkkdz.sHtML

[Q83] 大小写转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gxgsascdm.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gbryxqvhw.sHtML

[Q84] 去除首尾空格
来源：http://www.share.fanxiaobao.xyz/Article/details/gllxfxvrs.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gumzmgiex.sHtML

[Q85] 数值取整
来源：http://m.share.fanxiaobao.xyz/Article/details/gpzbvgdmu.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.fanxiaobao.xyz/Article/details/grmeassjr.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.fanxiaobao.xyz/Article/details/gdplttczx.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghlmyukef.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gghmtvpwb.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.fanxiaobao.xyz/Article/details/geqryrxep.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmxheexen.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fanxiaobao.xyz/Article/details/gmzjtvhbw.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gflmjnmfr.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdqbmhmyx.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.fanxiaobao.xyz/Article/details/gjsktxhun.sHtML

[Q90] 生成序号列
来源：http://blog.fanxiaobao.xyz/Article/details/grvammjtg.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.fanxiaobao.xyz/Article/details/gtwtkprbt.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/ggjogznvs.sHtML

R. Bash 专题
来源：http://read.share.fanxiaobao.xyz/Article/details/gyomugtwo.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gzdlzrqyl.sHtML

[R01] shebang 与严格模式
来源：http://mobile.fanxiaobao.xyz/Article/details/gwtrpzzoy.sHtML

#!/usr/bin/env bash
来源：http://www.blog.fanxiaobao.xyz/Article/details/grekwkamg.sHtML

set -euo pipefail
来源：http://www.m.share.fanxiaobao.xyz/Article/details/govynoovw.sHtML

[R02] 变量赋值与使用
来源：http://read.share.fanxiaobao.xyz/Article/details/guzblmmhh.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyuugvcgy.sHtML

[R03] 只读变量
来源：http://blog.fanxiaobao.xyz/Article/details/ghchosvcl.sHtML

readonly PI=3.14
来源：http://www.blog.fanxiaobao.xyz/Article/details/gshmqohxs.sHtML

[R04] 位置参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gujzzodtl.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.fanxiaobao.xyz/Article/details/gmljqybdz.sHtML

[R05] 参数默认值
来源：http://3g.fanxiaobao.xyz/Article/details/gulnagnjp.sHtML

name="${1:-default}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gvbnocjlf.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxjczaoqd.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gjbzoqrwy.sHtML

[R07] if 判断文件
来源：http://blog.fanxiaobao.xyz/Article/details/gkuduhyuq.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gjderqmbf.sHtML

[R08] 数值比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gybyqvjyu.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gvmtusxlc.sHtML

[R09] 字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/gzkuplent.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gbgtdohll.sHtML

[R10] 正则匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/gbgxbieye.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/glnakzduy.sHtML

[R11] case 多分支
来源：http://wap.fanxiaobao.xyz/Article/details/ggcuguobp.sHtML

case "$1" in
来源：http://m.share.fanxiaobao.xyz/Article/details/guxbecfja.sHtML

start) echo "启动" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gzzkiemma.sHtML

stop)  echo "停止" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gwrmvcnes.sHtML

*)     echo "未知命令" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gopgtgflu.sHtML

esac
来源：http://baike.fanxiaobao.xyz/Article/details/gwokqkeue.sHtML

[R12] for 遍历文件
来源：http://mobile.fanxiaobao.xyz/Article/details/guzqmcyqi.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gpvsonudc.sHtML

[R13] for 计数循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gvtswfyng.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gnwknvrjj.sHtML

[R14] C 风格 for
来源：http://m.share.fanxiaobao.xyz/Article/details/gzkaauapg.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gpuyxujik.sHtML

[R15] while 逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcvqiybkf.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/ggctpiuei.sHtML

[R16] until 等待条件
来源：http://wap.fanxiaobao.xyz/Article/details/gblmncrfb.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.fanxiaobao.xyz/Article/details/gxodgackc.sHtML

[R17] 数组定义与取值
来源：http://m.share.fanxiaobao.xyz/Article/details/gardtfyzc.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gkrnquurd.sHtML

[R18] 遍历数组
来源：http://wap.fanxiaobao.xyz/Article/details/gxaaymfoi.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gexsfxiri.sHtML

[R19] 数组长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gbhfelkgj.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpclnmgkv.sHtML

[R20] 关联数组（字典）
来源：http://www.share.fanxiaobao.xyz/Article/details/ggfohdfpx.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gmxzmzxfw.sHtML

[R21] 字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/giiqtyzjv.sHtML

echo "${#s}"
来源：http://read.share.fanxiaobao.xyz/Article/details/ggutrkada.sHtML

[R22] 截取子串
来源：http://blog.fanxiaobao.xyz/Article/details/gjvozlskj.sHtML

echo "${s:0:5}"
来源：http://mobile.fanxiaobao.xyz/Article/details/ggetijgzk.sHtML

[R23] 字符串替换
来源：http://www.share.fanxiaobao.xyz/Article/details/ghgwuehbs.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmhwjcmwo.sHtML

[R24] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/gkwuctybv.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.fanxiaobao.xyz/Article/details/gzsuaafqn.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtzljhxam.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.fanxiaobao.xyz/Article/details/ggmtcfmeb.sHtML

[R26] 命令替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glrhtnzao.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvjdebqzo.sHtML

[R27] 算术展开
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkhlieswe.sHtML

echo $((1 + 2 * 3))
来源：http://baike.fanxiaobao.xyz/Article/details/gjeyoccqh.sHtML

[R28] 浮点运算
来源：http://baike.fanxiaobao.xyz/Article/details/gfpyekuee.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gppksxlzb.sHtML

[R29] 定义函数
来源：http://blog.fanxiaobao.xyz/Article/details/gheuclhhk.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvizrkgpf.sHtML

[R30] 函数返回状态码
来源：http://blog.fanxiaobao.xyz/Article/details/girezbqqy.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.fanxiaobao.xyz/Article/details/ggxqhxqta.sHtML

[R31] 局部变量
来源：http://3g.fanxiaobao.xyz/Article/details/gutxepefe.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gyfmdnelv.sHtML

[R32] 参数个数校验
来源：http://blog.fanxiaobao.xyz/Article/details/grjjgoiha.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gilcmyrld.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gooedkpst.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.fanxiaobao.xyz/Article/details/gmkxxjgyg.sHtML

[R34] 退出时清理
来源：http://m.share.fanxiaobao.xyz/Article/details/grojgxnjc.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/geicwiyhb.sHtML

[R35] 后台执行并等待
来源：http://m.share.fanxiaobao.xyz/Article/details/gglsmmibf.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.fanxiaobao.xyz/Article/details/gvhfeaggm.sHtML

[R36] 并发执行多个任务
来源：http://m.share.fanxiaobao.xyz/Article/details/gqtdgswlq.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.fanxiaobao.xyz/Article/details/ggkzruhob.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/giqndseof.sHtML

files=$(ls -1)
来源：http://read.share.fanxiaobao.xyz/Article/details/glufdaiex.sHtML

[R38] 管道串联
来源：http://read.share.fanxiaobao.xyz/Article/details/gnllinjrc.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/guxobilqx.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geqfijwuo.sHtML

cmd > out.log 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gddienncf.sHtML

[R40] 追加写日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gkaavvhwo.sHtML

echo "log" >> out.log
来源：http://mobile.fanxiaobao.xyz/Article/details/ghenydjrd.sHtML

[R41] 丢弃输出
来源：http://baike.fanxiaobao.xyz/Article/details/gmuewzavm.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/gcjpdibrs.sHtML

[R42] 输入重定向
来源：http://wap.fanxiaobao.xyz/Article/details/ggkuponlu.sHtML

wc -l < a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gawwwlpds.sHtML

[R43] 按名字查找文件
来源：http://blog.fanxiaobao.xyz/Article/details/giklshuev.sHtML

find . -name "*.log" -type f
来源：http://3g.fanxiaobao.xyz/Article/details/gzleosxjg.sHtML

[R44] 按修改时间查找
来源：http://m.share.fanxiaobao.xyz/Article/details/gomcjrwrs.sHtML

find . -mtime -7 -type f
来源：http://3g.fanxiaobao.xyz/Article/details/gfmqquryy.sHtML

[R45] 批量删除
来源：http://blog.fanxiaobao.xyz/Article/details/ghksjdfwj.sHtML

find . -name "*.tmp" -delete
来源：http://3g.fanxiaobao.xyz/Article/details/guawfswua.sHtML

[R46] 递归替换文件内容
来源：http://3g.fanxiaobao.xyz/Article/details/gbugkwyfn.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fanxiaobao.xyz/Article/details/gxjxazzvt.sHtML

[R47] sed 单行替换
来源：http://3g.fanxiaobao.xyz/Article/details/giluqbddf.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsseqdurd.sHtML

[R48] awk 取指定列
来源：http://3g.fanxiaobao.xyz/Article/details/gwaoksdgt.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gcbepxodf.sHtML

[R49] awk 带条件
来源：http://3g.fanxiaobao.xyz/Article/details/gtwvvxywe.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fanxiaobao.xyz/Article/details/geicebkbl.sHtML

[R50] awk 求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gjbfkibnm.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gzhjcwrii.sHtML

[R51] 排序去重取前几
来源：http://mobile.fanxiaobao.xyz/Article/details/gigfxfrme.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.fanxiaobao.xyz/Article/details/gqkbwpykv.sHtML

[R52] 统计行数
来源：http://m.share.fanxiaobao.xyz/Article/details/gijqzvyer.sHtML

wc -l a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gffcubowy.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcqlcyeqo.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkmspksuh.sHtML

[R54] 比较两个文件
来源：http://wap.fanxiaobao.xyz/Article/details/gmqqkdhjg.sHtML

diff a.txt b.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gmighpzlj.sHtML

[R55] 压缩与解压
来源：http://wap.fanxiaobao.xyz/Article/details/gqiaturqk.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fanxiaobao.xyz/Article/details/gyhrzprvl.sHtML

[R56] 远程拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/ghghlccft.sHtML

scp file user@host:/path/
来源：http://read.share.fanxiaobao.xyz/Article/details/gpdtcihsi.sHtML

[R57] 远程执行命令
来源：http://3g.fanxiaobao.xyz/Article/details/gjnncgbdm.sHtML

ssh user@host 'uptime'
来源：http://mobile.fanxiaobao.xyz/Article/details/gwwdcvtdp.sHtML

[R58] 下载文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggqfrglig.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.fanxiaobao.xyz/Article/details/givullidi.sHtML

[R59] 发 POST JSON
来源：http://wap.fanxiaobao.xyz/Article/details/gcdtvmfhx.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/gttzjhaqv.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.fanxiaobao.xyz/Article/details/ghqymxpcu.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fanxiaobao.xyz/Article/details/gpkyyzhxt.sHtML

[R61] 磁盘占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzzvpqolc.sHtML

df -h;  du -sh *
来源：http://www.blog.fanxiaobao.xyz/Article/details/grcaqwpqd.sHtML

[R62] 找最占空间的文件
来源：http://3g.fanxiaobao.xyz/Article/details/gbhranvhw.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fanxiaobao.xyz/Article/details/grthfgpvb.sHtML

[R63] 内存与进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqqbebdda.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fanxiaobao.xyz/Article/details/gczcnngtk.sHtML

[R64] 结束进程
来源：http://read.share.fanxiaobao.xyz/Article/details/ghhgoaisx.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxhwhfifu.sHtML

[R65] 查看端口占用
来源：http://read.share.fanxiaobao.xyz/Article/details/gdyajuwdw.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fanxiaobao.xyz/Article/details/gjpnkdptx.sHtML

[R66] 定时任务
来源：http://m.share.fanxiaobao.xyz/Article/details/gbhjdugfr.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gipannpyi.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fanxiaobao.xyz/Article/details/gnasdvdyf.sHtML

openssl rand -hex 16
来源：http://blog.fanxiaobao.xyz/Article/details/gypjnmgnf.sHtML

[R68] 计算文件校验值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnpltjsox.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gjfsducvp.sHtML

[R69] 生成随机密码
来源：http://www.share.fanxiaobao.xyz/Article/details/gotggpqgj.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gddeibpzb.sHtML

[R70] 时间戳与互转
来源：http://m.share.fanxiaobao.xyz/Article/details/gjozupgbb.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.fanxiaobao.xyz/Article/details/gedmsxnba.sHtML

[R71] 日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvagdcqll.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpuunljqg.sHtML

[R72] 等待端口就绪
来源：http://m.share.fanxiaobao.xyz/Article/details/gejnajaai.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gqmgehzqo.sHtML

[R73] 分割大日志
来源：http://blog.fanxiaobao.xyz/Article/details/gawkygjta.sHtML

split -l 1000 big.log part_
来源：http://m.share.fanxiaobao.xyz/Article/details/gnffiwxhf.sHtML

[R74] 批量重命名
来源：http://blog.fanxiaobao.xyz/Article/details/gqfpnangl.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gixvawfqe.sHtML

[R75] 导出环境变量
来源：http://baike.fanxiaobao.xyz/Article/details/gsxtcccuk.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gppsrpxdt.sHtML

[R76] 使用临时文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gcwspsaff.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/gfkxinqma.sHtML

[R77] 读取用户输入
来源：http://wap.fanxiaobao.xyz/Article/details/gaqidlnkg.sHtML

read -rp "请输入: " ans
来源：http://3g.fanxiaobao.xyz/Article/details/gbsxtbhmx.sHtML

[R78] 交互式菜单
来源：http://m.share.fanxiaobao.xyz/Article/details/gltaksbbh.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.fanxiaobao.xyz/Article/details/gyecipkht.sHtML

[R79] 解析命令行选项
来源：http://baike.fanxiaobao.xyz/Article/details/giwqhjpnp.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.fanxiaobao.xyz/Article/details/gcylzvzlc.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.fanxiaobao.xyz/Article/details/gknyftlac.sHtML

time ./run.sh
来源：http://mobile.fanxiaobao.xyz/Article/details/giarftbng.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gkkaibrry.sHtML

S. C / C++ 专题
来源：http://mobile.fanxiaobao.xyz/Article/details/gppjuvmal.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/guvcpwfrx.sHtML

[S01] C：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gbrxwfuai.sHtML

#include <stdio.h>
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxdshpxhs.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.fanxiaobao.xyz/Article/details/gbbtpcdvw.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gntktbsjg.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fanxiaobao.xyz/Article/details/gouzhhdbi.sHtML

[S03] C：读入整数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzkoukfuu.sHtML

int x; scanf("%d", &x);
来源：http://baike.fanxiaobao.xyz/Article/details/gbuvyplos.sHtML

[S04] C：字符串复制
来源：http://m.share.fanxiaobao.xyz/Article/details/gjpgpewyw.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fanxiaobao.xyz/Article/details/gzfaabkoz.sHtML

[S05] C：字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/gzbkdwwqa.sHtML

strlen(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvolfqlxi.sHtML

[S06] C：字符串比较
来源：http://wap.fanxiaobao.xyz/Article/details/gtnkjsvit.sHtML

strcmp(a, b) == 0
来源：http://blog.fanxiaobao.xyz/Article/details/gspbrqozp.sHtML

[S07] C：数组遍历求和
来源：http://mobile.fanxiaobao.xyz/Article/details/ghqpxksxc.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fanxiaobao.xyz/Article/details/gecyrikpe.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxsteldeo.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.fanxiaobao.xyz/Article/details/gjmqhzlzw.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.fanxiaobao.xyz/Article/details/giqwbxelg.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.fanxiaobao.xyz/Article/details/gfqsnmkoj.sHtML

[S10] C：指针与解引用
来源：http://baike.fanxiaobao.xyz/Article/details/gmgljeuzg.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtofqokgb.sHtML

[S11] C：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gqngexmnq.sHtML


<!-- 参考信息 -->