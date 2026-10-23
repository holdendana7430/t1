代发 wailian999

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3rgooybae.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3xrccubiy.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3rrkomiom.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3reqggmos.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3mqmeerji.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3cluixkij.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3gcmpsdnp.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3nbqayhnb.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3wqelvnip.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3vxcvdujo.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3syclasxo.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3hyrsiicl.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3nnztexuw.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3iwycsvrt.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3qravdcra.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3oxxhayzy.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3wrvcrokr.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3grsumiux.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3kahgfclc.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3klmomuny.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3lahttfeh.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3gpuexrcg.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3yflmioir.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3dblxuyya.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3lobiibia.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3unggcszk.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3eihahvzu.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3yyzppdty.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3ujspuvyq.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3ffepemrc.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3drjrweqq.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3yeyekfit.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3sjhrpuqf.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3ovfsfwyi.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3skjlyngw.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3zeraaevv.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3eygbtlfr.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3sqbkyssx.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3jpzfvwdk.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3hgthdptx.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3phrndlsn.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3muixjefk.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3ubpdyotn.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3rfjupyvg.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3glpdpjtr.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3xhrtcium.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3jepcoqts.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3ckdjnxvr.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3cswjshrx.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3jribdgqh.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3kxdmngqk.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3umycnfon.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3nogvqysn.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3mlgyyxae.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3ikhssoop.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3ciuxvjmh.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3ybmzkdlc.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3bhcsqccb.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3kjspxjit.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3pioczevm.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3atifvbss.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3fpihxzbu.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3emdhrhip.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3iaqhikbm.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3lagveejq.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3zsjvelrm.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3autvmims.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3fznmtwbm.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tsonhbig.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3ahuwhjvk.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3qacfxfvo.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3yjoztnju.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3rkubrcpr.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3wjxxsvvp.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3qfeykyov.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3amicqzmq.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3xdgxtzjo.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3gfoislgr.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3goeqbeld.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3afdqjenb.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3aubrwpli.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3crcewpft.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3lqpeqreh.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3jpjvliec.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3xuvhyeuq.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rkxmywtj.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3vhucbfsc.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3cwbwapzq.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3djxsotsc.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ueraitdc.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3nvktbchx.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3klfiptgs.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3buzovizd.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vwibkwah.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3norsirkc.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3jjqgfijt.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3szbjfjdk.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3slqzkino.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3yjjetryj.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3fewcwzvx.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3squrbyik.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3oyhkbroy.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qqahsqjg.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3cvvbnshv.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3kvdwhqsr.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3iwdvjmzg.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3aafqzzih.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rkruiwwy.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3ggoevxsy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mdjuyjpz.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3wkbgivzf.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3jkzdkxwk.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3tcdnthwc.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3ojgbvmjr.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3cecxdedq.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3gvezmwwn.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3rkqyhjvy.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3cosuodjt.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3vuqrnpqq.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3dkmkbaty.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3mpjxwtdr.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3palygxkb.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3odjjlobi.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3muhdenqi.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3odjnhvto.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3uxuovgsc.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3pozuapyw.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3mhohihha.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3fxawbdav.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3cixakbzt.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3qebbnhss.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3tcipcrdl.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3euwgfwud.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3hvfidotj.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3bpwuwaws.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3fnrqhasi.html

esac
来源：http://www.52xcode.cn/Article/details/gt3dywnfadv.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3hzhwhgtu.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3qmbzibec.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3oymdzjxw.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3pphtglfc.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3crzsdpsu.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3nwtaquey.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3zqdiecwf.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3loczfqdl.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3gfaijrtz.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3dfbwixie.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3xorynlfw.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3lmbnrcjn.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3vzagunjc.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3dswnedzh.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3pbawjkby.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3sxsisntq.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3wpcgyaun.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3jgjgahjq.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3ljirmzmv.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3kfuzpcby.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3pepbwqst.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3jqdmysjz.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3zjkkskyi.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3ricairve.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3irwhkmjt.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3ezjercwn.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3afzuhdrw.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3adzpzmvh.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3clisuidm.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3hjofxwsm.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3fmgqhjev.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3btvjasov.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3nczeyadf.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3kdidnmis.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3dprhprmi.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3zkyypwpf.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3luuocxbp.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3dvxqnozm.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3sxishksr.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3nfkbwzuv.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3ktzsrmjc.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3cxcgashc.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3rwncgdpd.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3sfbxnwff.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3zxeqstpj.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3rnawxavd.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3esmkcvqy.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3xdfldbpi.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3oztgselh.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3fkwpqoxv.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3wnlvstum.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3wkmnbyad.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3nsnetkrj.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3hpxwdvmi.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3cxsjzzeq.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3ysimpxsg.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3fzofprhn.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3pbxgcmdj.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3udopipkn.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3ywzwcaez.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3jxhwfnbn.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3yqzthozf.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3izinxshg.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3ygowfiad.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3tvpwryts.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3zibjnxyh.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3pgrofscp.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3evskokfw.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3qhaqpjpo.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3qksxolrs.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3bdvetaak.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3gopyegzr.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3mavqwgma.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3hobmsfzl.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3drdhzcan.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3hdunnjtg.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3copryzrw.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3qdmsvoic.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3gikfkjct.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3vncpscds.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3evghnvtj.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3thwerwbp.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3penrxcpg.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3wqethzab.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3cxihzfmk.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3dojvnecy.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3kqsvyycg.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3pijllmpz.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3qxkmemxc.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3miyxeash.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3ejluvxtb.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3bkgzbkhb.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3kkzvrwil.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3tvoxihdj.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3bpiljezw.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3exruurfn.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3flhxlzab.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3drgbqdxz.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3ggxtsckm.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3gcgeolgy.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3iukbssbp.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3pwyazbki.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3fnowwafh.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3mqumgbix.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3felhcjzu.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3vgprmlpj.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3uywrfgac.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3wvxadafz.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3uadujuyx.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3tezpkess.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3xogxlxsd.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3pdtlpney.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3qcmnhotp.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3ddmaooza.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3skqrxhls.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3slxifrvk.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3lrwqyuhp.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3twydgpjk.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3npovxfwd.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3bqcdxqvc.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3chrrakoi.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3eqrucpuy.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3lrvwkwnw.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3yvftfowd.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3rmseckts.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3bcmmpjst.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3myxasewt.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3ndubufze.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3nnpcwcek.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3zxnqjudw.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3izvbuvuf.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3vcpgrinr.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3nlxjhyhx.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3kxwrakur.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3fdfipstu.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3bbejesur.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3vghxlswm.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3dtzfzscc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3grexlecf.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3tadzdrrf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gybugeve.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3cvetiyso.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3kxepmxbh.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3bmdsjvra.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3fvmldxpw.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3zjpagims.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3gybnemxy.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3tflqlwpj.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3xrfocabm.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3kscjummd.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3ciscabzm.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3sjqaomyl.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3opbhlvmu.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3arojszcm.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3eqpvnypb.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3odbeqsjt.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3yhlycfcr.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3srszcogq.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3qzarnqsl.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3ddficrxf.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3nhhnhlif.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3rtzyikbo.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3rsnnxzei.html


<!-- 参考信息 -->