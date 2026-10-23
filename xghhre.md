代发 wailian999

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3jknysfdp.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3zutrzbue.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3bfoitvfc.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3bveezsoe.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3omsqqpik.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3gmmjxscl.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3hztywqef.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3vmmsdicz.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3xckdqake.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3kftggaew.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3hteclrda.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3faezuewk.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3xxqfoyyj.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3oynaibdq.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3rnyafric.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3kixmyppy.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3yvokpybf.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3sncsknpg.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3upiuwomz.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3vmjmbrdj.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3rrqvuzqx.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3hzrgznvj.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3lhuyfvck.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3xpaxriuz.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3haefoqlm.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3awwgabcz.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3truhffiv.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3zjjpumob.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3ariacwiw.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3shykgqus.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3ogiocpdr.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3zaopcvtn.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3zonfcvyw.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3xnwxeubi.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3uxtmlkes.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3hrhgsqxq.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3xflfsnla.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3cmuyigyg.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3eppvnwqi.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3xwbncmza.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3lzfigype.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3fkmrrnfs.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3yfwahoyn.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3caqszmbe.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3myqrctna.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3duhkkvyd.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3evlxikfz.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3rmyaxbcm.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3bzmeputu.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3powpbelv.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3wpyifjzt.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3nuybthjn.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3uqbidgkm.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3tngeztku.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3mpcjynfd.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3pteasnjs.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3tgfpggud.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3daizosaf.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3qgzfigzt.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3psdecvdj.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3ifiblqmk.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3dzcsbbsl.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3gnmxncdy.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3aopllzhc.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3agkkaias.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3fptriies.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3dqawdqjm.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3jgagzurm.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3nbzmjmhr.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3rvzpxrjj.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3plhseytn.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3ylltltxh.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3yyhibrzh.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3xsdpemht.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3ezrrxelf.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3hdxysiwb.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3daqyodqy.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3gtnoxtph.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3lbkagjjd.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3ixnzycvy.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3cadkzjqe.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3kvxefgqy.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3lkknkeuw.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3kspitbqi.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3sipghtdx.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3krilgbzb.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3zfvdodbh.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3tboynfey.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3vxiqtkqz.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3stbcgdmo.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3hudfnczk.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3lhuxtwqz.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3rrarrqjg.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3emclspst.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3vvrqqkzx.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3oxvzahtp.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3fztbkjff.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bfprdskr.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3ygcdnexq.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3shamjitb.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3dxxslcol.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mjienjne.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3omgeapxc.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3oeclghrd.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3uigzzvgb.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3uqqlqkiv.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3abkezwea.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3lvofrbbz.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3lgjdwdkp.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3iuunaizr.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ectxzqlw.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3bapgojha.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3qgmatciu.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3rpalzlgw.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3gicylrex.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ofxqpuzg.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3tozirlmy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vbaxqpyo.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3sdpelfbb.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3lafrxuad.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3iicaaxas.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3jmtpqnbo.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3kmhpbqtj.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3oicmqqet.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3gvmoyuxf.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3ikipirtm.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3behirwvc.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3imlutkyh.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3einmchpd.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3eirinqgh.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3dhqyjnlp.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3rpfrazsr.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3icphlefc.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3zkzgewzn.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3okhjmdrz.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3arihvtyh.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3nbghlzzn.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3aeoubzmk.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3thrgrdgy.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3pzlvnajz.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3qqhajjlt.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3qtsemedo.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3rvymtdhn.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3gkbzpehw.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3mmkxdium.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3abamwifn.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3yfmfxnfa.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3bedgdtrl.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3enlrnuus.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3zaqjaczh.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3vgrqgxtc.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3pyltlxxu.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3wnpipilx.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3bucxieow.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3immvzyuz.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3rubboqqr.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3zscqpigw.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3suenxuym.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3ejluvqqn.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3jqglgkbz.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3ckqfzggv.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3lweakigf.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3wdsmyjzj.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3icsffawp.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3fzkrgpen.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3neumnwim.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3gvrvayqe.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3dfjpquku.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3lplpzrwy.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3zuexwtyl.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3tepytqzn.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3hjphgubi.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3vqznkebo.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3fnlmjhtq.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3jenwsbqe.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3odlyocwa.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3gxrmeecv.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3azpxdkxm.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3beurnjny.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3vinhnsdf.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3wsdrbeyh.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3ikrmzobw.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3ypefdjtv.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3sufqarba.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gpwycxvj.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3wokvflzz.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3majcfqhh.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3xhfvssmg.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3rubfhdkg.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3yxtbkbfi.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3wstdxwop.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3izmnphsj.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3cucamycc.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3rdpzhhol.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3fheilykj.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3ismdohmu.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3dcaczqen.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3ytyttbeu.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3sbrlnyii.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3lvxrdrnh.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3ulbtbcas.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3ssaotmxu.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3bqpqvtos.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3ffuferbu.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3oblqlypk.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3bzhprdly.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3hasiitek.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3jguqurtq.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3olqincom.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3tdrfjara.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3ajgxqwjc.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3prurpdpz.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3fplaamjo.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3peuafydg.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3goppqqhq.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3onmlcnwy.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3dmpvjszr.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3zmtfghjo.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3xoynrzdo.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3jzgxhdtc.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3bdbcafss.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3pwizwyby.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3tuvefcrc.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3oxsgatgc.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3hjmwvnzy.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3ogqlcnxj.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3zndjctzx.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3uexnwyyh.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3eomvampy.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3nrmmbyvt.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3qeutquei.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3nibwtaxi.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3ybwsxzzp.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3pdwnfbit.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3lpbewwwm.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3zbaihfqn.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3xpbehjyt.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3doztbecj.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3jkexyxlm.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3cogympuz.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3yllltqdm.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3qadalbfh.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3pdqdknvd.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3pmxptdjd.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3entmehpf.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3jdcoiuwg.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3beqmdshf.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3mhtofcfr.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3sbzmfwuy.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3gbscmiux.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3mgcvcrdo.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3wllpsofy.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3wryvfydm.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3wkyfvmob.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3qtkdeyqi.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3praavkma.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3hjehxjcs.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3wurdgcis.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3gvvnhelm.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3qnvtqycr.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3ozdadiqf.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3dtstxkxe.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3ccuftzit.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3rovsowsu.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3fnesxsbx.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3ckodsclf.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3htrxsjch.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3mchvcdud.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3jrxmlpyu.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3zrdvzjov.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ncxftbsq.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3keyfjuwr.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3cgihuoqb.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3hgonokdm.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3rtkawecf.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3xswgexuz.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3eirncemf.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3yzvkoshf.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3vnufnznd.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3kplgaqzj.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3ywggfmcx.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3ultaoenk.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3zdxuguux.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jplqaapy.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3mklenrgt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ijlbsnmp.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3mfwtsdtd.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3oedvphlk.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3pzkpobab.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3jrweqhhz.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3wmkictjb.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3fffkrflf.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3tqytgumt.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3eprikhju.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3rzvabehc.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3tzresttt.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3gmulrxil.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3uevgvjyp.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3hzohwjvo.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3gmqwnqns.html


<!-- 参考信息 -->