代发 wailian999

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2laeynifm.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2xeewonik.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2xrykfdhy.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2oviecdbc.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2dbwhqqqp.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2ihsxxvof.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2kqliyynw.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2qbnttgkr.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2hcbkgjra.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2qinlhcnh.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2eucgwrdd.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2qooshreg.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2fxdsswgj.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2nceesedi.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2nfubdhwx.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2apagzyau.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2cnuvzjhh.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2fejgmuji.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2nnwvrjge.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2jqadmxqm.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2plnsnmcw.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2pexyypwm.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2xpunfigm.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2lmnqakwx.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2qflcidwg.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2uctimxtw.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2maujgrsf.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2vfwwhwxq.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2yakcffie.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2rpyeeefo.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2mngzuvlf.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2cdhlrehj.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2anbcmwje.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2bweggdgg.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2uzulnfdn.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2faxzmuft.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2iltxrqax.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2oshkqzea.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2prsyptlb.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2hleeepfi.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2pnoozkpx.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2bmqsxbzs.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2pttinpav.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2mglkufzf.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qyjlatow.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2wwjzjnwm.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2onqjmnyp.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2dmrjxqfd.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2eikbusic.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2ddjthtwy.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2whenkppc.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2mymqmshs.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2glukbmrc.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ddhmziiq.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2kmqrwild.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2ysgfxldu.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2pxpbqqdi.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2gutrljfz.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2vhmjnmnd.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2npmxmjvd.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2gataahad.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2twcnlshj.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2znxnlxbs.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2apqosier.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2zaogtajs.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2rgninbdm.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2jeizmugd.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2gbvshpvp.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2ysvduyiq.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2mdpduqng.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2dlgvtpfb.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2hmsffjdw.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2mlspodkk.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2yvtjzagk.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2xkxkzntx.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2twjmqjic.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gnttosmh.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2rowdmgpw.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2icxbisdr.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2webybizi.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2rwmlpdqa.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2bobxkkoh.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2gzrugjqa.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2vqvshuqn.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2zvcyhhzm.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2pavueqbm.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2ujxvcxtu.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2uuapoxuu.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2sjzpscyo.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2tcmvxjja.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2enbbuksw.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2uemfiuzp.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2mifcnkar.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2oaaxzeuw.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2ndtdvavd.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ggkiurwx.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2rnerxnrk.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qppwrcsj.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2xvykshjk.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2npqknflv.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2nriqivyj.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2givhiflv.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2ahanvvgf.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2lvycobya.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2cvkycdlv.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2erqbuesu.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2oebviipw.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2gtsayora.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2tcotujff.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2ffqcxfqr.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zajwsfsj.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2oicakxar.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2ckwyqlcm.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2paeothgt.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2sdwcqmwf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qlhgnmjl.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2glfmnyss.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bzgtewdr.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2ybhfqhxa.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2byrgulac.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2gtwkckwy.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2xrkvxqpu.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2tggmyars.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2xylohpvh.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2uusrcobo.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2zrezespk.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2iswxmsre.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2nnycspfj.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2bqatwcid.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2bhxjuuiw.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2qsniqdkx.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2sjicusys.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2jplrlbqw.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2pwjzbfbg.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2dwjdoaqk.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2ttfhzswi.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2rcwnrnjn.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2ivsfbpyk.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2hdvompkc.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2muhnbyjw.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2iyvufjhz.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2pxuxygci.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2udzqofsk.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2fdzgsasl.html

esac
来源：http://www.52xcode.cn/Article/details/gt2gmpehogt.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2esktdszv.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2iqmfwnkg.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2oyctmyzm.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2vtsudmto.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2hxwebvap.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2hjalaayd.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2jnlsctrt.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2dkmlnxpu.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2yzgahkxo.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2zoaknuwb.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2lnwqgtbz.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2vwkivzmk.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2vjflgmco.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2oysnisit.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2ukjhhifv.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2hwldzmbw.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2ornbkdce.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2yykwjdzn.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2wxzwlkvt.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2kxyouehl.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2xixiglhg.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2aezfnkrx.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2icviberb.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2zfmfsubt.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2jfjjxvnq.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2wgcpcgou.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2qmswvwsz.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2txmxdkmj.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2auprlrir.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2sjztroda.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2ghbiwiqd.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2gkoakfgg.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2ihitetnm.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2rencvxkh.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2jddyyosy.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2zqfvidxj.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2fdfftvpp.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2rndmwjxc.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2exbrglaa.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2yxeffvyc.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2aqptvklz.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2blgdyghm.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2yhymndto.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2eusndzdj.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2aaypqebk.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2ehezypdk.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2ujdgsmhi.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2znrcgdve.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2viqdgxtb.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2wpkrjwla.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2extaogwn.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2bxnfqehe.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2haqckuky.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2lkzctjqf.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2bzdmhwtp.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2jgahsumc.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2dhylvzde.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2bjhxkjui.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2jrvvryig.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2cccoukci.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2ijfvvuwt.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2fshbzlmt.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2kpbmmhlr.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2evxeqnip.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2cmujmoou.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2wmsvjoxl.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2dsaggwnh.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2qnohqqmr.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2wpvhhtft.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2ezkeseya.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2qocajahw.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2ybkoasta.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2llnedsoe.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2gnccuazd.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2dqnhefwu.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2dcwhpzvl.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2ujyfntuc.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2upekbccd.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2raufksgg.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2kqrqfqkf.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2fyonnmki.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2nfbgdqvn.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2khqqhzhi.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2zfagcyco.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2tyhcdxfi.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2vuogxwnx.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2mskjgefz.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2edhwrnqx.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2tzlczwor.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2dybzbkpo.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2jfamdzcv.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2ywhdbazs.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2vrlzquoc.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2kqzphvor.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2whnvxhrp.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2yjpyxknk.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2xetstlyn.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2annvrlgd.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2sdkuftdm.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2bzbhexru.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2glxjpftg.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2chvisjjj.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2rdelfxvq.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2qvrxmatj.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2hqxyyvkz.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2xmpslqnv.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2zrqcpcus.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2psasclri.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2ytfrqbgz.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2lbeufhfh.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2tyntuqxo.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2cqadocci.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2ayfzekxi.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2daiffdhd.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2taejhtid.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2pzevvngw.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2tqizkgfm.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2ovryyctl.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2wewakuaj.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2asvlnqds.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2otyjjzct.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2rvjjbtpp.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2ieojrukr.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2pvvfoklp.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2gykoulqs.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2sbfimata.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2kmslkpcc.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2wjxrbjij.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2jatwimba.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2xjbhmygb.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2ljmajosw.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2mplbfqnw.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2zkuxyejz.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2esfrendg.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2mhssuumu.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2ojjstrgv.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2acbchaqx.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2pbtigbgh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qfeyttyg.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2bfacadez.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xlvdhseu.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2gwzyoesp.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2lqnvgdbe.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2tvelapvs.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2axgfqbbe.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2tkljsxcf.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2haiyzfyw.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2kwrbqglt.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2paxawqdu.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2phytbwkk.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2bgekakzc.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2lqjfjhjp.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2bzellnpt.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2cqfmjpwo.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2tjlybqmp.html


<!-- 参考信息 -->