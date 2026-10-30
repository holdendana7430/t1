代发 wailian999

SELECT u.name, o.amount FROM users u
来源：http://www.share.fehbvm.com/Article/details/ghrkfvccs.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.zdbjq.cn/Article/details/gphshskpb.sHtML

[Q43] 标量子查询
来源：http://wap.hesvh.cn/Article/details/gysuayfoo.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.fehbvm.com/Article/details/gmfaemcut.sHtML

[Q44] IN 子查询
来源：http://baike.fehbvm.com/Article/details/gastftbdy.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.zdbjq.cn/Article/details/gdspjpfbp.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.fehbvm.com/Article/details/gqlvsajzg.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.hesvh.cn/Article/details/gygnhxqmf.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.fehbvm.com/Article/details/gjnwcsglx.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fehbvm.com/Article/details/gupvtlflj.sHtML

[Q47] 与平均值比较
来源：http://m.share.zdbjq.cn/Article/details/gdwuqvzgq.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.hesvh.cn/Article/details/gnjmcufxi.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.fehbvm.com/Article/details/gjesthosc.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.zdbjq.cn/Article/details/ggnfpaevt.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.fehbvm.com/Article/details/gumagajzf.sHtML

[Q49] 更新单行
来源：http://www.m.share.zdbjq.cn/Article/details/glpnghmxj.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.fehbvm.com/Article/details/girzkfvqs.sHtML

[Q50] 批量更新
来源：http://3g.zdbjq.cn/Article/details/gjpzcecaf.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.hesvh.cn/Article/details/gxbqxqdeh.sHtML

[Q51] 用子查询更新
来源：http://www.share.hesvh.cn/Article/details/ghvvfljuo.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.zdbjq.cn/Article/details/gzvzupakb.sHtML

[Q52] 删除指定行
来源：http://m.share.fehbvm.com/Article/details/gzzoftxhh.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.zdbjq.cn/Article/details/gerbpqdyd.sHtML

[Q53] 按条件删除
来源：http://www.m.share.fehbvm.com/Article/details/guusyhsjr.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.hesvh.cn/Article/details/gftdiiuhk.sHtML

[Q54] 清空表
来源：http://baike.hesvh.cn/Article/details/gxyweopss.sHtML

TRUNCATE TABLE logs;
来源：http://baike.hesvh.cn/Article/details/gevreoxme.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.hesvh.cn/Article/details/gyybtsale.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.fehbvm.com/Article/details/gehqvqlaa.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.fehbvm.com/Article/details/gnanpefgq.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.fehbvm.com/Article/details/ggjznemvn.sHtML

[Q57] 行号
来源：http://3g.fehbvm.com/Article/details/gmtcksvuj.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.zdbjq.cn/Article/details/ghnwwmlwk.sHtML

[Q58] 累计求和
来源：http://www.share.zdbjq.cn/Article/details/giwzohnqq.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.hesvh.cn/Article/details/ggmbbfzbf.sHtML

[Q59] 分组内累计
来源：http://read.share.zdbjq.cn/Article/details/gcawqpwnf.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gygqqfscs.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.hesvh.cn/Article/details/gcojltxoo.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.zdbjq.cn/Article/details/gruafjdru.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gaogmfgfp.sHtML

[Q61] 移动平均
来源：http://3g.fehbvm.com/Article/details/gujjwkmsg.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.zdbjq.cn/Article/details/ggcquwumz.sHtML

[Q62] 分组占比
来源：http://www.blog.zdbjq.cn/Article/details/grhcudiqf.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.zdbjq.cn/Article/details/gtqdnnacd.sHtML

[Q63] 开启事务
来源：http://www.blog.fehbvm.com/Article/details/gtxflrtlh.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.zdbjq.cn/Article/details/gapwbxrhp.sHtML

[Q64] 提交事务
来源：http://blog.fehbvm.com/Article/details/gbinucxvz.sHtML

COMMIT;
来源：http://wap.zdbjq.cn/Article/details/gdluruhne.sHtML

[Q65] 回滚事务
来源：http://blog.hesvh.cn/Article/details/gwuesmmwm.sHtML

ROLLBACK;
来源：http://3g.zdbjq.cn/Article/details/gqywkvnjt.sHtML

[Q66] 行锁查询
来源：http://3g.zdbjq.cn/Article/details/gxgltqcta.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.fehbvm.com/Article/details/gclqroijv.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.zdbjq.cn/Article/details/gefhucklh.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.zdbjq.cn/Article/details/gmorutlua.sHtML

[Q68] 保存点
来源：http://read.share.zdbjq.cn/Article/details/gdwttkgle.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.zdbjq.cn/Article/details/gjqkjoqrt.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.fehbvm.com/Article/details/gafiletcc.sHtML

[Q69] 查看执行计划
来源：http://mobile.fehbvm.com/Article/details/gbqwbgwpg.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.fehbvm.com/Article/details/gktzfvcxe.sHtML

[Q70] 更新统计信息
来源：http://read.share.hesvh.cn/Article/details/gleofvzau.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.fehbvm.com/Article/details/ggvlvckko.sHtML

[Q71] 查看建表语句
来源：http://3g.hesvh.cn/Article/details/gcdsvdixh.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.zdbjq.cn/Article/details/gpwsmqjog.sHtML

[Q72] 查看索引
来源：http://mobile.fehbvm.com/Article/details/ghybaopvh.sHtML

SHOW INDEX FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gexurcebw.sHtML

[Q73] 查看表状态
来源：http://mobile.zdbjq.cn/Article/details/gwvjfzjcd.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.zdbjq.cn/Article/details/guumjymxw.sHtML

[Q74] 强制使用索引
来源：http://mobile.zdbjq.cn/Article/details/gdvtkkjkz.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.zdbjq.cn/Article/details/gfioriljk.sHtML

[Q75] 日期格式化
来源：http://read.share.fehbvm.com/Article/details/gqxfyrlmi.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.fehbvm.com/Article/details/gtodgvevn.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.hesvh.cn/Article/details/ggcxzwexq.sHtML

[Q76] 按天统计
来源：http://mobile.zdbjq.cn/Article/details/gkdfsvubi.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.zdbjq.cn/Article/details/gbvaargmn.sHtML

[Q77] 时间加减
来源：http://3g.zdbjq.cn/Article/details/gmeliohbf.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.fehbvm.com/Article/details/gztuxjtgt.sHtML

[Q78] 当前时间
来源：http://www.blog.hesvh.cn/Article/details/gbymkjwvk.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.fehbvm.com/Article/details/grsiyyinn.sHtML

[Q79] 字符串拼接
来源：http://blog.hesvh.cn/Article/details/ggutuvqtm.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.fehbvm.com/Article/details/ggeqyavhf.sHtML

[Q80] 字符串截取
来源：http://www.blog.zdbjq.cn/Article/details/gsbjtynma.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.fehbvm.com/Article/details/gvgxzqqaj.sHtML

[Q81] 字符串替换
来源：http://baike.fehbvm.com/Article/details/geonorezf.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.hesvh.cn/Article/details/gqnpxunvz.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.fehbvm.com/Article/details/gcdtpmsmd.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gpakzxsyg.sHtML

[Q83] 大小写转换
来源：http://www.blog.hesvh.cn/Article/details/gkpdadjkr.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gkeozjklc.sHtML

[Q84] 去除首尾空格
来源：http://m.share.zdbjq.cn/Article/details/gxdripmye.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gpdbnhzqt.sHtML

[Q85] 数值取整
来源：http://www.m.share.fehbvm.com/Article/details/gxwyhnsdw.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.fehbvm.com/Article/details/gyhmvblvs.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.fehbvm.com/Article/details/gwtfryjpj.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.hesvh.cn/Article/details/gnmwfaqjv.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.hesvh.cn/Article/details/gcrmsjhjx.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.fehbvm.com/Article/details/gmtegpokj.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.hesvh.cn/Article/details/gmdfvupuk.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.zdbjq.cn/Article/details/gdcsatcpf.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gbqteunmu.sHtML

[Q89] 判断表是否存在
来源：http://blog.hesvh.cn/Article/details/gfkhohswt.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.zdbjq.cn/Article/details/galnovodb.sHtML

[Q90] 生成序号列
来源：http://wap.fehbvm.com/Article/details/gdjxcoyzx.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.zdbjq.cn/Article/details/gmmboxhnh.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gklyiujdt.sHtML

R. Bash 专题
来源：http://www.m.share.hesvh.cn/Article/details/gcuxfepbv.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gzbexzbfd.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.fehbvm.com/Article/details/gzcrgtwsy.sHtML

#!/usr/bin/env bash
来源：http://baike.zdbjq.cn/Article/details/greciuhyl.sHtML

set -euo pipefail
来源：http://read.share.fehbvm.com/Article/details/gyrjblusu.sHtML

[R02] 变量赋值与使用
来源：http://mobile.hesvh.cn/Article/details/gamvqzktf.sHtML

name="Tom"; echo "$name"
来源：http://wap.fehbvm.com/Article/details/gsyvrlcmm.sHtML

[R03] 只读变量
来源：http://baike.zdbjq.cn/Article/details/gewekqmkd.sHtML

readonly PI=3.14
来源：http://wap.fehbvm.com/Article/details/gngaammzj.sHtML

[R04] 位置参数
来源：http://blog.zdbjq.cn/Article/details/gzvyltxgi.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.zdbjq.cn/Article/details/gonxtkvrv.sHtML

[R05] 参数默认值
来源：http://read.share.zdbjq.cn/Article/details/gmnogktsz.sHtML

name="${1:-default}"
来源：http://mobile.zdbjq.cn/Article/details/groqdnnap.sHtML

[R06] 判断命令是否存在
来源：http://mobile.zdbjq.cn/Article/details/gelafkply.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.fehbvm.com/Article/details/glhjkkgrf.sHtML

[R07] if 判断文件
来源：http://read.share.zdbjq.cn/Article/details/gsietqtqh.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.fehbvm.com/Article/details/grhlhpvrn.sHtML

[R08] 数值比较
来源：http://wap.zdbjq.cn/Article/details/gyxjyiakn.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.hesvh.cn/Article/details/gmrlnlumf.sHtML

[R09] 字符串比较
来源：http://3g.hesvh.cn/Article/details/gmthztqtu.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.hesvh.cn/Article/details/gvipdpefu.sHtML

[R10] 正则匹配
来源：http://wap.zdbjq.cn/Article/details/gpptnlrxr.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gxgakbrdo.sHtML

[R11] case 多分支
来源：http://wap.fehbvm.com/Article/details/gydsjzquh.sHtML

case "$1" in
来源：http://www.m.share.hesvh.cn/Article/details/gewfjwrit.sHtML

start) echo "启动" ;;
来源：http://3g.fehbvm.com/Article/details/goxmhgius.sHtML

stop)  echo "停止" ;;
来源：http://m.share.fehbvm.com/Article/details/gdrysfouc.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.zdbjq.cn/Article/details/ggpvbqmdp.sHtML

esac
来源：http://read.share.zdbjq.cn/Article/details/gfnxvrigo.sHtML

[R12] for 遍历文件
来源：http://www.share.hesvh.cn/Article/details/gmvsrgbdv.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.zdbjq.cn/Article/details/gnfcuqoow.sHtML

[R13] for 计数循环
来源：http://www.share.hesvh.cn/Article/details/gytqzgckf.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.zdbjq.cn/Article/details/gvovwkbge.sHtML

[R14] C 风格 for
来源：http://www.blog.fehbvm.com/Article/details/gpwksqpjr.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.fehbvm.com/Article/details/gegfgwecs.sHtML

[R15] while 逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gylidscvx.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.fehbvm.com/Article/details/gulkqchrg.sHtML

[R16] until 等待条件
来源：http://mobile.hesvh.cn/Article/details/gpfxwhrzl.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.hesvh.cn/Article/details/grrqzqawu.sHtML

[R17] 数组定义与取值
来源：http://3g.fehbvm.com/Article/details/ghajhcanw.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.zdbjq.cn/Article/details/gklcmstly.sHtML

[R18] 遍历数组
来源：http://3g.hesvh.cn/Article/details/glscvkrjn.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.fehbvm.com/Article/details/gypubuvjj.sHtML

[R19] 数组长度
来源：http://read.share.fehbvm.com/Article/details/gdimrpjrh.sHtML

echo "${#arr[@]}"
来源：http://3g.zdbjq.cn/Article/details/gyrrnwbwl.sHtML

[R20] 关联数组（字典）
来源：http://read.share.hesvh.cn/Article/details/gloukcdsu.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.hesvh.cn/Article/details/gphdvaxri.sHtML

[R21] 字符串长度
来源：http://wap.fehbvm.com/Article/details/ggzbgojjw.sHtML

echo "${#s}"
来源：http://m.share.fehbvm.com/Article/details/gqqsheuwe.sHtML

[R22] 截取子串
来源：http://www.m.share.fehbvm.com/Article/details/gdqiwqvbx.sHtML

echo "${s:0:5}"
来源：http://baike.hesvh.cn/Article/details/gwpdgsrbk.sHtML

[R23] 字符串替换
来源：http://www.m.share.fehbvm.com/Article/details/gxrmdybvu.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.hesvh.cn/Article/details/gktadduat.sHtML

[R24] 大小写转换
来源：http://3g.zdbjq.cn/Article/details/guysfqvlu.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fehbvm.com/Article/details/gklyqywvh.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.zdbjq.cn/Article/details/galzfespe.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.hesvh.cn/Article/details/gvhskvijw.sHtML

[R26] 命令替换
来源：http://www.blog.zdbjq.cn/Article/details/gxazqrflb.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.zdbjq.cn/Article/details/gfunafran.sHtML

[R27] 算术展开
来源：http://wap.fehbvm.com/Article/details/gobmfutgk.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.hesvh.cn/Article/details/gfqpejpze.sHtML

[R28] 浮点运算
来源：http://3g.hesvh.cn/Article/details/gshlrokas.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.hesvh.cn/Article/details/giojlkill.sHtML

[R29] 定义函数
来源：http://wap.zdbjq.cn/Article/details/gmmxifbko.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.hesvh.cn/Article/details/gcrxvouvp.sHtML

[R30] 函数返回状态码
来源：http://baike.zdbjq.cn/Article/details/gqsdktrri.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.zdbjq.cn/Article/details/ghsqgsnjd.sHtML

[R31] 局部变量
来源：http://3g.zdbjq.cn/Article/details/gqamsgceh.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.hesvh.cn/Article/details/gaejuupoy.sHtML

[R32] 参数个数校验
来源：http://read.share.zdbjq.cn/Article/details/gnoxaypzs.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.fehbvm.com/Article/details/gswedpqof.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.fehbvm.com/Article/details/gqmxpgqoq.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.fehbvm.com/Article/details/gbpflayco.sHtML

[R34] 退出时清理
来源：http://mobile.zdbjq.cn/Article/details/gpzqyuxqe.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fehbvm.com/Article/details/gfilclzdo.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.zdbjq.cn/Article/details/gnwgjrkmj.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.zdbjq.cn/Article/details/gqgksjjzm.sHtML

[R36] 并发执行多个任务
来源：http://wap.fehbvm.com/Article/details/gfplxmwyj.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.fehbvm.com/Article/details/gymzatnkp.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.fehbvm.com/Article/details/gbaacrrpa.sHtML

files=$(ls -1)
来源：http://blog.hesvh.cn/Article/details/ggqzacjmi.sHtML

[R38] 管道串联
来源：http://mobile.hesvh.cn/Article/details/gdtiesooj.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.hesvh.cn/Article/details/ganwpmajc.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.zdbjq.cn/Article/details/gfckbiffn.sHtML

cmd > out.log 2>&1
来源：http://m.share.zdbjq.cn/Article/details/glyouzalh.sHtML

[R40] 追加写日志
来源：http://www.blog.hesvh.cn/Article/details/grmighais.sHtML

echo "log" >> out.log
来源：http://3g.fehbvm.com/Article/details/gweonaupq.sHtML

[R41] 丢弃输出
来源：http://blog.zdbjq.cn/Article/details/gkcsxyxpi.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fehbvm.com/Article/details/gsqtoqahu.sHtML

[R42] 输入重定向
来源：http://3g.hesvh.cn/Article/details/guhwepcup.sHtML

wc -l < a.txt
来源：http://www.share.hesvh.cn/Article/details/gskzlqdzz.sHtML

[R43] 按名字查找文件
来源：http://blog.zdbjq.cn/Article/details/gbnrwyoyn.sHtML

find . -name "*.log" -type f
来源：http://blog.hesvh.cn/Article/details/gwnsvovsj.sHtML

[R44] 按修改时间查找
来源：http://mobile.zdbjq.cn/Article/details/gurswcxls.sHtML

find . -mtime -7 -type f
来源：http://3g.fehbvm.com/Article/details/gxvfrfyim.sHtML

[R45] 批量删除
来源：http://www.blog.zdbjq.cn/Article/details/gzbagaucy.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.zdbjq.cn/Article/details/gconlixvh.sHtML

[R46] 递归替换文件内容
来源：http://baike.fehbvm.com/Article/details/gdpetwgmz.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.fehbvm.com/Article/details/gohpbgtht.sHtML

[R47] sed 单行替换
来源：http://baike.hesvh.cn/Article/details/galbdyaao.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.zdbjq.cn/Article/details/gookeisnf.sHtML

[R48] awk 取指定列
来源：http://m.share.fehbvm.com/Article/details/gsfpbzqvs.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.zdbjq.cn/Article/details/gerpbnvnh.sHtML

[R49] awk 带条件
来源：http://www.share.hesvh.cn/Article/details/grvflqfzm.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.zdbjq.cn/Article/details/gxihkgxjn.sHtML

[R50] awk 求和
来源：http://www.m.share.fehbvm.com/Article/details/gtstmdhiq.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.hesvh.cn/Article/details/gdguqyeyw.sHtML

[R51] 排序去重取前几
来源：http://baike.fehbvm.com/Article/details/guahmyopt.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.hesvh.cn/Article/details/gsnloxamw.sHtML

[R52] 统计行数
来源：http://www.share.zdbjq.cn/Article/details/gdfkeymiv.sHtML

wc -l a.txt
来源：http://m.share.hesvh.cn/Article/details/gqbynotxn.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.fehbvm.com/Article/details/gvnurubms.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.fehbvm.com/Article/details/gdofdfxox.sHtML

[R54] 比较两个文件
来源：http://blog.zdbjq.cn/Article/details/gzlsuzlms.sHtML

diff a.txt b.txt
来源：http://mobile.hesvh.cn/Article/details/gzfomungk.sHtML

[R55] 压缩与解压
来源：http://read.share.fehbvm.com/Article/details/gietivklo.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.hesvh.cn/Article/details/gjzeikaaz.sHtML

[R56] 远程拷贝
来源：http://baike.fehbvm.com/Article/details/gmymgwbhp.sHtML

scp file user@host:/path/
来源：http://www.blog.fehbvm.com/Article/details/gxuzccstm.sHtML

[R57] 远程执行命令
来源：http://baike.hesvh.cn/Article/details/gipfsugqi.sHtML

ssh user@host 'uptime'
来源：http://m.share.hesvh.cn/Article/details/gcakmkxpy.sHtML

[R58] 下载文件
来源：http://www.blog.fehbvm.com/Article/details/gghicdfcw.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.zdbjq.cn/Article/details/gagnvnyce.sHtML

[R59] 发 POST JSON
来源：http://m.share.fehbvm.com/Article/details/ghcbltqfz.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.hesvh.cn/Article/details/gclyzuzww.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.hesvh.cn/Article/details/gvwwypvol.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.hesvh.cn/Article/details/gzmulredc.sHtML

[R61] 磁盘占用
来源：http://read.share.fehbvm.com/Article/details/ggnfbtrrp.sHtML

df -h;  du -sh *
来源：http://read.share.zdbjq.cn/Article/details/gcrjaqsyw.sHtML

[R62] 找最占空间的文件
来源：http://wap.zdbjq.cn/Article/details/gacxqdpnv.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.fehbvm.com/Article/details/gryzqhojy.sHtML

[R63] 内存与进程
来源：http://m.share.hesvh.cn/Article/details/gnndvvtxm.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fehbvm.com/Article/details/gpczdegkr.sHtML

[R64] 结束进程
来源：http://baike.zdbjq.cn/Article/details/grlprseqp.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.hesvh.cn/Article/details/gvzxqfqeo.sHtML

[R65] 查看端口占用
来源：http://blog.fehbvm.com/Article/details/gweunfdmd.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.fehbvm.com/Article/details/gspxukeqi.sHtML

[R66] 定时任务
来源：http://www.m.share.hesvh.cn/Article/details/gffxtqqkb.sHtML

crontab -e;  crontab -l
来源：http://baike.zdbjq.cn/Article/details/gbtxcvbpn.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.hesvh.cn/Article/details/gjeyzhdek.sHtML

openssl rand -hex 16
来源：http://3g.zdbjq.cn/Article/details/gaaiezdck.sHtML

[R68] 计算文件校验值
来源：http://mobile.zdbjq.cn/Article/details/grdqalyxa.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.hesvh.cn/Article/details/gvjjefwdu.sHtML

[R69] 生成随机密码
来源：http://m.share.zdbjq.cn/Article/details/gmmxhnaza.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.zdbjq.cn/Article/details/gwljbnwss.sHtML

[R70] 时间戳与互转
来源：http://baike.zdbjq.cn/Article/details/gybcdxkqo.sHtML

date +%s;  date -d @1700000000
来源：http://3g.hesvh.cn/Article/details/gpkyecuob.sHtML

[R71] 日期格式化
来源：http://3g.zdbjq.cn/Article/details/gxuuabuxz.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.hesvh.cn/Article/details/gemftskne.sHtML

[R72] 等待端口就绪
来源：http://3g.zdbjq.cn/Article/details/gbjatsznq.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.hesvh.cn/Article/details/gqudnjvvt.sHtML

[R73] 分割大日志
来源：http://3g.fehbvm.com/Article/details/ghxtydmuo.sHtML

split -l 1000 big.log part_
来源：http://m.share.fehbvm.com/Article/details/gcscmaaxe.sHtML

[R74] 批量重命名
来源：http://baike.zdbjq.cn/Article/details/gxaiqjspc.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.zdbjq.cn/Article/details/gnxujslpp.sHtML

[R75] 导出环境变量
来源：http://www.m.share.hesvh.cn/Article/details/gduynuzwj.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.zdbjq.cn/Article/details/gyrxxnzmr.sHtML

[R76] 使用临时文件
来源：http://baike.fehbvm.com/Article/details/gnuozgybd.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.hesvh.cn/Article/details/ggvhprvko.sHtML

[R77] 读取用户输入
来源：http://3g.fehbvm.com/Article/details/gmumbatiu.sHtML

read -rp "请输入: " ans
来源：http://read.share.fehbvm.com/Article/details/grxfkylfo.sHtML

[R78] 交互式菜单
来源：http://3g.hesvh.cn/Article/details/gsowtmuwi.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.hesvh.cn/Article/details/ghkuzrkpt.sHtML

[R79] 解析命令行选项
来源：http://www.share.fehbvm.com/Article/details/glgtelxar.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.hesvh.cn/Article/details/gekfjnxvt.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.hesvh.cn/Article/details/gefnhyozl.sHtML

time ./run.sh
来源：http://m.share.zdbjq.cn/Article/details/gmrfgpfep.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gzmqzffnx.sHtML

S. C / C++ 专题
来源：http://baike.hesvh.cn/Article/details/gcnwpxebz.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/ganyfejfg.sHtML

[S01] C：Hello World
来源：http://wap.fehbvm.com/Article/details/glwtkxqnm.sHtML

#include <stdio.h>
来源：http://www.blog.hesvh.cn/Article/details/gmlfpkqqd.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.fehbvm.com/Article/details/gngjqdqwj.sHtML

[S02] C：变量与格式化输出
来源：http://blog.zdbjq.cn/Article/details/gqdjrktwc.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.zdbjq.cn/Article/details/gfeqmgvja.sHtML

[S03] C：读入整数
来源：http://wap.zdbjq.cn/Article/details/gsvoktxtd.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.hesvh.cn/Article/details/gctbrsuso.sHtML

[S04] C：字符串复制
来源：http://3g.hesvh.cn/Article/details/ghtgcvyqw.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.zdbjq.cn/Article/details/gxirwlhvk.sHtML

[S05] C：字符串长度
来源：http://read.share.zdbjq.cn/Article/details/gdxmhsejw.sHtML

strlen(s)
来源：http://blog.fehbvm.com/Article/details/gdynngcwv.sHtML

[S06] C：字符串比较
来源：http://www.blog.fehbvm.com/Article/details/gsixlupas.sHtML

strcmp(a, b) == 0
来源：http://www.blog.zdbjq.cn/Article/details/gcitznmpf.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fehbvm.com/Article/details/ggpnwvhvk.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.hesvh.cn/Article/details/gsalcvrbh.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.hesvh.cn/Article/details/gsmhtnayc.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.zdbjq.cn/Article/details/gghplwinn.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.hesvh.cn/Article/details/ghhywupyg.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.fehbvm.com/Article/details/giacbvnkj.sHtML

[S10] C：指针与解引用
来源：http://m.share.fehbvm.com/Article/details/gocblqclm.sHtML

int *p = &a;  *p = 5;
来源：http://baike.zdbjq.cn/Article/details/ggtvelria.sHtML

[S11] C：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gyqkaffud.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.hesvh.cn/Article/details/gibieqzvx.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.hesvh.cn/Article/details/gzjlorvkw.sHtML

fclose(f);
来源：http://blog.zdbjq.cn/Article/details/guctlbocq.sHtML

[S12] C：写文件
来源：http://baike.zdbjq.cn/Article/details/gyxcxlqsu.sHtML


<!-- 参考信息 -->