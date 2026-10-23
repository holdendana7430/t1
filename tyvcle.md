代发 wailian999

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3mfspklax.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3gbyysxym.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3cdivtvnm.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3unpfpeds.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3nijhqlwo.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3pmhecicg.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3noaawpmf.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3avipualj.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3hyctnpaa.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3jrklroyb.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3jigfbtjb.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3rzjbwozc.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3rehclvfv.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3zjkfnxlp.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3fbikalxv.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3bhhoktzt.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3avsnjvkk.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3qpjfebce.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3urihhzmp.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3gqertchg.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3atgszsae.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3ixscchsg.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3yhhswnvr.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3nenybkhs.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3jmgtbnna.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3exellzfp.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3hfzdluwx.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3knvkrenm.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3pbfvqmen.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3lkdlxxuc.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3snpddyzs.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3cqlqulah.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3fnsmtkzi.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3abcrwpgz.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3enedukyk.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3kmzsxeqz.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3plobuosf.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3ofosmfkx.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3gsypssdz.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3skzlkqyb.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hiamxvri.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3nrymfhlv.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3hiieemvh.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3vnvfyfvj.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3gvlzmdvv.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3pkvepwwr.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3zwwrktly.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3hccuzxkk.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3idkuyrqx.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3kocszmrt.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3kazkaaui.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3sclohcug.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3bhqkbtzh.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3zchjjkwa.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3avvxmwlj.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3iolbcvka.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3ngulgdud.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3rawggatd.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3arhkxhif.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3nwozbmlz.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3aebllplv.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3nemeeldl.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3etuzcxde.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3ofgnywxs.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3bzirrnmq.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3yggxbfdn.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3sggihiwn.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3ixuuienf.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3lkmhiagl.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3ddxwchjh.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3itcdbuha.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3uzvroazg.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3abckzvsi.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3hwoxbjxc.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3invtsujd.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3vhsaxzgv.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3kiojwnga.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3ggdiarvi.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3qwkzdqes.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3dugmrojj.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3kxehjktq.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3duuwxcpj.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3fgzbjesh.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3ouqmanmx.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3nrmtmpyc.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3fqfgfklc.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3xyzjvptm.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3kadksihu.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3oqkhmaww.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gywalsbb.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3zgnwrhnb.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rhwnmgje.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3hziswotk.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zataoqno.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3exigoqpv.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3uhlalkxm.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3xwdfmxuy.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kannqwyk.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3tikzqbwb.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3mstskyhu.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3xendklhu.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3oczrrtnu.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3cvcynokj.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3oaaogeya.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3etgtwgla.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3qaoszxwl.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gzgnatod.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3nffjyygt.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3mgcjmmvf.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3vvpzjzay.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3ksapvsxq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lglrkqad.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3lrbjvytd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3labapdwa.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3wohkqyct.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3mdwricyv.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3bwhpyewq.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3cdlekzhl.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3veaeygvs.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3eiumyxnx.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3zfjboioo.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3rfiphaqw.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3gihaodtn.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3kpdfcokj.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3jkwfokai.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3cyiqybbi.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3asexedxe.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3ytnfckdv.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3gkavqqie.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3pyrcfpdo.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3djfckqky.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3wicdbqey.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3hjgiherl.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3dkakwphw.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3twrreces.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3guponpso.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3posymdfo.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3vvxzlztn.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3rigodhpb.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3nzpuakxa.html

esac
来源：http://www.52xcode.cn/Article/details/gt3orzgdihs.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3pcxfbtvr.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3hxafkkxw.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3qtcmbqug.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3rzobkque.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3dkmebgnv.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3dxfbwdci.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3sgrsthod.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3hpvncxgs.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3pvqkyoog.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3ndeixipk.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3vchddoon.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3zpqtimqm.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3smorroot.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3vnbklrpc.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3xnkxljjb.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3vlxmjvxz.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3zzpharcx.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3vlwhqexk.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3aivbdixp.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3ngwcbksw.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3wqllzqjf.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3serzplgf.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3nzbjeybk.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3jyrzeflz.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3cxixaabv.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3luszhegp.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3lvttwhlw.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3yshnihme.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3irraomrm.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3udqblfrn.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3mhbqojmk.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3lcgrujlp.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3regvmxnd.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3ulldemxz.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3hnndcopl.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3chnlkjsj.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3hrxnihwg.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3rodltqfi.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3lsywqvbp.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fbxhfbyr.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3wwckihog.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3fwobenac.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3sbgusjtb.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3zrlcgcic.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3aqynansi.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3osgbmaji.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3urtaflgt.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3edjolghp.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3ttfwrtdb.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3cqkudius.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3tawjtpzl.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3cbmacyjz.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3bfbphcxe.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3ahxatcij.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3flydeqqq.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3idzlusda.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3ujstzxkm.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3wxdubtuy.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3cpgfnpeh.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3uiiscugl.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3aslwjipt.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3kwqcycdx.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3omitplnd.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3ldxoojea.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3kcbzwuku.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3wqtftaot.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3dmlwtbru.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3voyenlgd.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3zqagszdi.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3aunenrkk.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3zkusbbkq.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ultezzbe.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3wqtibdmq.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3nzporsdn.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3vyyqdkww.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3ktbfzjcx.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3gannrlrs.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3axsvztiw.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3iglrpxkx.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3zlupypjp.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3vyhrxrff.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3xnochdvz.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3hixdmrhb.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3xnixpbll.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3uekurddk.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3kntkbxtd.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3qqaujbgw.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3xodgbqwq.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3oqlykapp.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3dobcgmkk.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3syimtdmp.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3eqbqjyjb.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3fydgpyua.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3rwsidajn.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3emretxaq.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3jakxtohh.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3sbhiyyqk.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3ictaiclj.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3cdcnnpvq.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3mimfwyqd.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3jlkeajxu.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3gkpozmer.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3swwijbxy.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3odmeuzcm.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3cmnxvzhf.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3pepwftzw.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3xpykpjgv.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3vysnpmvz.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3vsfkbubz.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3mnvyaduu.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3ykmusrkw.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3cghhjnqy.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3cfghdrgg.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3olrowawx.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3tfnfvqmb.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3bzznzplb.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3mijpkmlu.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3xceqqosm.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ouohibdh.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3dznewdnd.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3brlyzogt.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3zgkljewo.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3hrdprecr.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3qaarkydm.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3saxhvmdm.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3iknytneq.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3hnhvjyjg.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3jqzvatvh.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3osjlckrl.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3cidiymiq.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3rtqmgcky.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3gtukcksd.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3vtjhjrmw.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3filtzein.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3igulixse.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3hvfzyilh.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3objiabsw.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3mfokyqib.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3asyhrsrw.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3juptlndn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nrxqtycs.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3fsmmlwak.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3egdirpdt.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3hohfvaas.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3ucrkjidr.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3ewezmxjt.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3xfpcevfp.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3grgtbqck.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3etwplsps.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3uygjzlnr.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3djvjsswg.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mrraciso.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3hrmsaizo.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3plxwapjh.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3kjblxwjo.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3nolfklrs.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3qksfygpe.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3nbdbrgyc.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3ldwkjfzz.html


<!-- 参考信息 -->