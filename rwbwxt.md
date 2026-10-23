代发 wailian999

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3rrnqjrli.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3enzqiqok.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3ncmgorik.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3cdflpavc.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3jkagfmme.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3uzflkoxv.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3udeoqtxc.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3ynizlyqw.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3wxdtyuyg.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3kjskziov.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3ocbizsux.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3dsspjqmv.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3takzfgwa.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3atwrhife.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3oiahlypu.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3nlfitcoy.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3wesrvkcw.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3noxeamlu.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3tsmftmgy.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3ebfxrzhh.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3swtmrqih.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3ystmuhht.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3dpocqrgp.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3cuuvjrtl.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3fiaflihg.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3fgpobzqc.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3gupzpuvz.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3hwawgbwy.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3ghfbhreb.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3synruksu.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3wbkjwslg.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3qxtacgte.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3mcfyjtep.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3isnbhyie.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3fiqgripo.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3wmgbdoaw.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3tgayvzbi.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3aknfquuw.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3kbejqqlr.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3celymidg.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3vjkdfwpq.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3bjsicyep.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3csbvsguj.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3hjzrfrde.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3vbxhfezg.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3ypjbtxau.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3vlzmqmzl.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3vqvxkmkq.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gvnxkufe.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3ibxhznbx.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3dtkdaaoa.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3zrjzxvbz.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ccqeezac.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3afxjakyw.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3gtrzoeba.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3zjpfuzks.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3ajcbnhdr.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3jqyytndt.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3kjlntnpc.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3rpkyyihh.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3qatciuyf.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3mtztdtyj.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3bqtyplzx.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3vfoslxyt.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3vswlbtqy.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3ybfthvmf.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3bzxzbzcq.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3tbfrrwkq.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3whuaeoga.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3nuypdiiu.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3qgdlrjnx.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3schrxqmu.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3wwygsuoj.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3nbcxhqsb.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3udtyirij.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3baixkvfq.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3hyydvisk.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3wewkluwf.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3ietzytnu.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3umjdkake.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ptjltsqh.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3miuxlhny.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3ruovdlsd.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3samhbkbb.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3xyuofkfx.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3lwvfmubd.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3zdgqwurm.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3bceorbai.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3cdsoqabi.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3jgactzei.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3lbmfmvdl.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3kjrymiml.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3swrywwtu.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3hixrfoil.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3dgfnhkqo.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3lvyljqwr.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3bymjbjsl.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gjsevjws.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3nombjrhj.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nruhflox.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3ggmpxfez.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rzkfdgdb.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3ckxcuruz.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3fwyyeeqj.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3nvrjvqyw.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3illusatv.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3mlockxuh.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3zyarifiz.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3nywyreqe.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3wzfzxevx.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3xaemumqb.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3hjhnkimh.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3sgisuaed.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3dfmbofuh.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3tgwrhptr.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3hfvldpnc.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3iszctdsi.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3yxkzwktr.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3lhorgkzn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jzpddjwi.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3joomyozh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jbmkhlyi.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3wdfnnpxl.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3tmaomotd.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3cuuzjtmu.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3zgmmtiqd.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3tuuqbbyi.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3uumtwziz.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3wanhmwlb.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3xuklofuq.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3eapilhyj.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3wmuzthym.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3mprbijmx.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3prvkeuwd.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3uptfkqif.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3izkokyfy.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3jkuojrho.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3hbhyouib.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3yeeilgps.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3ijzmkhbq.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3wpvlgxgg.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3pggkjwpk.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3pedlmbpx.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3rpkeefyw.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3qqnjvild.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3nnmkmodd.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3gjkushft.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3kwefbuvj.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3xiccutrv.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3jssukvtx.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ztlhvghw.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3iqijopsx.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3kpwpdoyr.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3nxebibkr.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3gxburixb.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3pcjoducd.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3xdwbldvu.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3scyxvejz.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3penggbzi.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3zfhmwcih.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3fkkeeogv.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3orkbnagf.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3khwnarow.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3btkdlrcj.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3klkwbels.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3dgftbhqe.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3iiiqfupq.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3xseikhkr.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3cvlitwzd.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3kjabrohg.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3wutghzyn.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3flkyrrkb.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3qrpzbzsm.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3oqloeqbg.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3rmenhvxa.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3qdnnznrz.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3fvthzuuz.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3hkwftpwo.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3badyzaxo.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3nlayfvep.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3dfufgnuq.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3bdjqdumb.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3hdgcbozg.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3bigsfflt.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3vyjpbbxa.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3cqibvpug.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3ucpckhhs.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3kaahjgph.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3xnhxfovq.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3cpitbsmg.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3uixcsewj.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3ipyvxhys.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3fhjvnjjh.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3xvtdpmzq.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3xbqkqtzw.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3djapvhdi.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3nbhwmibj.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3vdiqmprh.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3jzooqfvp.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3ippprpng.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3zceqoupl.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3zvbmtgtj.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3wrvbryud.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3jwntnwfx.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3cfpldich.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3kvjcvfcb.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3zsggbpma.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3kkvrdxfq.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3hkxgtwew.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3trfqmhqt.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3dtencvrq.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3booocshh.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3fblhdpon.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3kppxkmtu.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3tovidypo.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3iaojaosh.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3haqlcsai.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3hvumrgmt.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3mcgumpaq.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3iuthswcf.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3ixifrcsv.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3qwwpecqn.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3yequnfjq.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3gmbnyewu.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3ynddhvjt.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3apyedsdz.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3lsoztfoh.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3trhqtmnj.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3nqpltjyo.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3zvmeckdj.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ntwqtmwl.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3qiaumwex.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3sgvltzxc.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3eqbodmei.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ariehnfd.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3ksakxxsc.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3auqojamm.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3ufalxeek.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3fxyilbcq.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3poembktn.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3ttkomwla.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3dkupnemh.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3vvkeacjd.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3bkuokixl.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3rtkkthog.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3qnwdxtvf.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3eaujjnln.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3lpmgoumw.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3axfpvgqn.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3tszbdrtx.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3pmofovbe.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3fbbmjjsp.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3dqpbawqm.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3lvhpzyne.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3xhldqjek.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3eqezhufc.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3jyjatcqw.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3phfexxcy.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3raleepks.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3uhjlxatg.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3cdeevpul.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3dtuadqlt.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3xdrvccqf.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3ftwfyqzw.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3obicmmae.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3rzcunpjj.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3qrcsvdgl.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3wrbkzdes.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3hzhbwcam.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3ouxktwrd.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3droljfnj.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3xuxqvdyj.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3unjhinsa.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3etrpbbbe.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3cqdaeusk.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3ixzqsggf.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3gvtusgsf.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3lmflxvrw.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3fsjlwcqr.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3hukyjhno.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3flsqewqv.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3djwbzksg.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3hdzpmegu.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3yhcrvish.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3oixpuwli.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3gwufdnrx.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3bfbbmwtu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bupoudil.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3olyzkqgd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mmaqqypf.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3kooaqkdp.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3twvnzsdz.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3dwokyvli.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3ryczswcv.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3qxnnygmv.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3wfdrkezd.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3hsntrrqt.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3sbbtkziq.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3audkesdh.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3osjwbzvd.html


<!-- 参考信息 -->