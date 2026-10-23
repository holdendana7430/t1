代发 wailian999

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3fzkhqvad.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3dxeuauhg.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3abfwsluo.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3uohyhcqa.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3oufbjhue.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3lcbsvpys.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3smxmfkme.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3bnmsvhmk.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3agoncztc.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3viwozhcw.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3ddasferh.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3sibgpuuq.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3zkwsndhb.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3vuqxzjat.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3dtditqey.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3jexpmrxt.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3mfehmqwq.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3mdulajvc.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3gigeuivn.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3dygvojgr.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3pgvgilea.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3lzupmcuy.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3exvryaha.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3bkybdgiz.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3vcpshcuj.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3cbnuhsjj.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3rekrlycm.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3hbazbnql.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ihlvhvia.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3rpxuyvfk.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3wlfjqsgl.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3snhanjfr.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3mkapgbwy.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3ulkpntvx.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3zhiyxcmd.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3giammpcp.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3jocqbftp.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3waewjbmm.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3crtwoxyr.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3podkukgh.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3yylngcod.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3nhyqeohm.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3glfonmni.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3znfubzjq.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3dshkdygv.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3wqnazelx.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3xilgtfez.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3pajlhusz.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3kilnzate.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3phtqwnfn.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3bnozgyrt.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3edugdveg.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3xqymkomy.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3jjedtvna.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3wchkkuwy.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3auognntc.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3hhxeuhiq.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3dnrlaibl.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3bnsdqzxn.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3ultgswks.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3mmzaomsq.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3lrwstfxy.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3doykheuo.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3vmjktbgf.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3vpxnaaan.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3wykzteub.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3cpdicctt.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3btyqdxdb.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3rlhfntgs.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3euwlnjad.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3ayqlzcfa.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3dktvxkcm.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wqxjmvdi.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3nhhzyhsd.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3zyvpylro.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3kidthwom.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3hwkkejkn.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3oaiiucrz.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3zbuebkfv.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3uaybtpvp.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3eafknpij.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3jlxbudrx.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3ywnvmrvw.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3gbfxfukl.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3qyysmghd.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3otxstahs.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3towmgpwb.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3slhkpmuh.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3ppaumfhx.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3eiatzdou.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3fufdexbo.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kinxesfs.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3syyodwib.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gceynbra.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3hazxfnqc.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qkxlqidl.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3lvkrhwen.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3johhvlaw.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3lhqwxhpx.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3vcylmrso.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3tjlscffg.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3deprmuep.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3ewqxepce.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3cqrthszn.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3gkcsxhfi.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3asvtiqbc.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mgazhecc.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3ojlkymfv.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3ipvxcrqz.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3cxjdutog.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3kdtdsxxx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kfbpcggt.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3epyigrpl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iolqxivo.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3uxnhyftg.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3uerkbpvs.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3kpoznylz.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3wriizofc.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3wusyeqgi.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3svnlmqru.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3vlblksax.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3wepsjief.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3intmsfyb.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3ygnqwprg.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3wqibbtjg.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3idehekvn.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3aerjdrfu.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3qyjlklgz.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3slxadvgf.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3xtyrurwv.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3yghgaxee.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3sqecrsvs.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3gntmvfuq.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3gimjcqah.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3umorucvp.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3mzbzyjvz.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3ufhqdtgd.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3xeytziaf.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3emnpbgtw.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3kqdtidye.html

esac
来源：http://www.52xcode.cn/Article/details/gt3pdqnjoos.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3otpncuvy.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3fdpmetnw.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3gesudaiw.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3nsrotggi.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3aciypfmx.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3egoxsaab.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3jwawbsfx.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3hscyzalx.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3qojawwmk.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3nwjadusc.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3ktrpdzoi.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3zispapyp.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3kjmamtix.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3rerxzliw.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3xmbatjow.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3vvhctoln.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3aozeopmw.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3nbmwleis.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3jjlfemor.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3pjkdfvgg.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3sytcjuyw.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3mimpkppq.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3fqmxnaus.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3xehjprhw.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3dgzqztmd.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3kmiiwbvr.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3mepsfcbp.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3usiodjcu.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3pgcouyif.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3jauzqbxi.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3dbaxegkf.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3rwtlaanc.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3dvpbjtcm.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3iggbrlxj.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3zmvdgakt.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3rlwtquob.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3ltbzrnwm.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3ncskiizd.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3kesiflku.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mbyjlkhv.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3zpadhclu.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3qygggkxy.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3xdzszeyn.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3aqtgtkxn.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3yicuvivn.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3vwasmtyn.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3kgnnsvyk.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3qjiwihyp.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3flfwlcwk.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3tpbjidal.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3lfrnvngs.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3ujmxotdx.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3nnvbxgsf.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3xwnfmamj.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3lffnzwfc.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3cyqkhnhs.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3frpykgbo.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3esccuijw.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3vxrzttwg.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3tfsxwxsa.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3zkywjrcb.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3lecfkrsz.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3aspvbxgp.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3isawxlno.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3sjzsrwya.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3morbpuke.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3dgohqsvt.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3itybctek.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3jyrbvkaq.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3pwsknjul.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3nfnojwts.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3lbilweut.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3iqkulxqf.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3qyamftvm.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3hjlqfwul.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3qipdtsyz.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3iorpbaqt.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3gosqjuys.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3olwefndy.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3krnuwzmw.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3ffwicguy.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3eckybfpg.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3kedjkkuc.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3khjmdvbg.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3dgxzshzw.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3wgrjguux.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3mczhurgi.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3cnxiuogc.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3eendvxhw.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3gppqmxbr.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3yrixizgn.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3alnawhxn.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3pwvwdcis.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3qyofxpzq.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3hxzgoeuc.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3imtsucep.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3mbafpcwb.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3vzpaasgq.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3datpcvrl.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3qpyewpke.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3ntxwsmur.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3zgvmdwgd.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3khojpihy.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3foovzbai.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3nvlpmdus.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3wiqtyqua.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3bfezqvzi.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3ogxemsyk.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3mddkxgbx.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3oggxhgnt.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3vwjuojwd.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3oqdyyotz.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3bxqoikye.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3oziwtgen.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3ikjxsmli.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3pcrvsxmu.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3smdahvpm.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3nufdbdpv.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3wiiwscrw.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3gkfzhvam.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3aplaofro.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3pyvgeyth.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3gmvdtbtx.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3uwqmehrr.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3vliaemwl.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3dazpynvf.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3jkoduxux.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3kpdqfhrd.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3quswpxch.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3dfsvwznj.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3mwcjpvqx.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3vbxdahkt.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3ymixkrud.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3ihgnifno.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3jonojcbk.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3dqxgxwik.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3fvgkfgxx.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3diybreuz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ksacpify.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3tseoiuzi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cayeftau.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3hkglmmxt.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3wmbmitsf.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3yibvirrp.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3oiugiqfr.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3kwnjzpjo.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3twcmdngc.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3zrykdulx.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3ogbzeiet.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3sbjyfqvu.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3cqlqzpig.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3bldpripd.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3bscgfkkk.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3srtdfghv.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3mnzlamir.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3cssdcbbf.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3xemydmyr.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3qhlcdonq.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3guydsjwf.html


<!-- 参考信息 -->