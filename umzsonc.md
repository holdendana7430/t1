代发 wailian999

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.fehbvm.com/Article/details/gjknhwgqc.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.hesvh.cn/Article/details/gdksxgzuo.sHtML

[Q47] 与平均值比较
来源：http://baike.hesvh.cn/Article/details/golzleqlu.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.fehbvm.com/Article/details/gnjvgdvge.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.hesvh.cn/Article/details/gjpmdyuqm.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.hesvh.cn/Article/details/gihwmfmya.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.fehbvm.com/Article/details/gihufbvzz.sHtML

[Q49] 更新单行
来源：http://blog.fehbvm.com/Article/details/gxzgvrbul.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.hesvh.cn/Article/details/gjkksjzun.sHtML

[Q50] 批量更新
来源：http://www.m.share.fehbvm.com/Article/details/gadapqjmm.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.zdbjq.cn/Article/details/gipnyfpeb.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.fehbvm.com/Article/details/gzkbfvygt.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.fehbvm.com/Article/details/gqwnprkga.sHtML

[Q52] 删除指定行
来源：http://baike.hesvh.cn/Article/details/gebowyhcn.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.fehbvm.com/Article/details/gdkqzxasq.sHtML

[Q53] 按条件删除
来源：http://www.share.fehbvm.com/Article/details/grtofwmxp.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.zdbjq.cn/Article/details/gjyzauubj.sHtML

[Q54] 清空表
来源：http://mobile.fehbvm.com/Article/details/ghhqppzvi.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.fehbvm.com/Article/details/ghlreqalq.sHtML

[Q55] 排名（并列占位）
来源：http://baike.fehbvm.com/Article/details/gzvwoaygs.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.zdbjq.cn/Article/details/gnwlcelfx.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.hesvh.cn/Article/details/glqaonahd.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.zdbjq.cn/Article/details/gfhrhzkad.sHtML

[Q57] 行号
来源：http://www.blog.fehbvm.com/Article/details/gulwmceaw.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.fehbvm.com/Article/details/gdzebaicf.sHtML

[Q58] 累计求和
来源：http://mobile.fehbvm.com/Article/details/gdincllpj.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gqvsygqxr.sHtML

[Q59] 分组内累计
来源：http://m.share.zdbjq.cn/Article/details/grwemjbjd.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gcpteatou.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.zdbjq.cn/Article/details/gvigauzff.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.fehbvm.com/Article/details/gagdpmwmq.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.fehbvm.com/Article/details/gsrhcfmmo.sHtML

[Q61] 移动平均
来源：http://baike.zdbjq.cn/Article/details/grbiinvhx.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.fehbvm.com/Article/details/grahdyaxc.sHtML

[Q62] 分组占比
来源：http://www.blog.hesvh.cn/Article/details/grosobpty.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.fehbvm.com/Article/details/gzylfbgeh.sHtML

[Q63] 开启事务
来源：http://www.m.share.zdbjq.cn/Article/details/ghasvpvft.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.zdbjq.cn/Article/details/gzvaasyti.sHtML

[Q64] 提交事务
来源：http://m.share.hesvh.cn/Article/details/gdmikgghe.sHtML

COMMIT;
来源：http://www.m.share.hesvh.cn/Article/details/gqktcwyna.sHtML

[Q65] 回滚事务
来源：http://mobile.hesvh.cn/Article/details/gicnajean.sHtML

ROLLBACK;
来源：http://blog.zdbjq.cn/Article/details/ghwjhayun.sHtML

[Q66] 行锁查询
来源：http://wap.hesvh.cn/Article/details/goafgqhjn.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.zdbjq.cn/Article/details/ghendhqsf.sHtML

[Q67] 设置隔离级别
来源：http://blog.zdbjq.cn/Article/details/gjldjjfey.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.fehbvm.com/Article/details/gzucmwvfa.sHtML

[Q68] 保存点
来源：http://read.share.zdbjq.cn/Article/details/gnsyuyufr.sHtML

SAVEPOINT sp1;
来源：http://www.share.fehbvm.com/Article/details/ggzojgtxc.sHtML

ROLLBACK TO sp1;
来源：http://baike.zdbjq.cn/Article/details/gnjzgwvzk.sHtML

[Q69] 查看执行计划
来源：http://read.share.fehbvm.com/Article/details/geiqaxrgj.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.fehbvm.com/Article/details/gtvsnoegk.sHtML

[Q70] 更新统计信息
来源：http://www.blog.fehbvm.com/Article/details/gkuufflrz.sHtML

ANALYZE TABLE users;
来源：http://www.share.fehbvm.com/Article/details/gyujuoico.sHtML

[Q71] 查看建表语句
来源：http://wap.hesvh.cn/Article/details/gzuzpttri.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.zdbjq.cn/Article/details/gcuchvavg.sHtML

[Q72] 查看索引
来源：http://wap.zdbjq.cn/Article/details/gjmnynoxy.sHtML

SHOW INDEX FROM users;
来源：http://3g.zdbjq.cn/Article/details/gdnmzfzim.sHtML

[Q73] 查看表状态
来源：http://read.share.fehbvm.com/Article/details/garwwxipb.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.zdbjq.cn/Article/details/gkkyicmea.sHtML

[Q74] 强制使用索引
来源：http://www.share.hesvh.cn/Article/details/glmfwvaak.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.zdbjq.cn/Article/details/gignclnjs.sHtML

[Q75] 日期格式化
来源：http://read.share.zdbjq.cn/Article/details/gmkctwklc.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.hesvh.cn/Article/details/garsbqych.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.fehbvm.com/Article/details/gbxzvdzzr.sHtML

[Q76] 按天统计
来源：http://wap.hesvh.cn/Article/details/ginoqzznr.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.hesvh.cn/Article/details/gqshpyqtl.sHtML

[Q77] 时间加减
来源：http://m.share.hesvh.cn/Article/details/gsxrwvxiz.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.hesvh.cn/Article/details/gtsiszmow.sHtML

[Q78] 当前时间
来源：http://3g.fehbvm.com/Article/details/gcnxcuzfk.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.fehbvm.com/Article/details/gdeozbspo.sHtML

[Q79] 字符串拼接
来源：http://read.share.hesvh.cn/Article/details/gcsgemvwi.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.hesvh.cn/Article/details/gtfjjkmex.sHtML

[Q80] 字符串截取
来源：http://read.share.hesvh.cn/Article/details/gitkdfloh.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.hesvh.cn/Article/details/guazycxfu.sHtML

[Q81] 字符串替换
来源：http://www.blog.zdbjq.cn/Article/details/gevdjgytl.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gsjosonlt.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.zdbjq.cn/Article/details/gmyqmamzr.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gfsvkqdnz.sHtML

[Q83] 大小写转换
来源：http://mobile.fehbvm.com/Article/details/gmxqpacxa.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gevfzhdvu.sHtML

[Q84] 去除首尾空格
来源：http://mobile.hesvh.cn/Article/details/gzxukwtqt.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gfekjiyhf.sHtML

[Q85] 数值取整
来源：http://3g.zdbjq.cn/Article/details/gwoybksuw.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.fehbvm.com/Article/details/gydgkkfha.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.zdbjq.cn/Article/details/gjnihebkq.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.hesvh.cn/Article/details/gmxlhiejp.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.hesvh.cn/Article/details/gbyfhmjdl.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.fehbvm.com/Article/details/gpxjhyzcm.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.fehbvm.com/Article/details/gkvybjcjb.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.hesvh.cn/Article/details/gijipcgav.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.fehbvm.com/Article/details/ghhrmzkod.sHtML

[Q89] 判断表是否存在
来源：http://wap.hesvh.cn/Article/details/gfkiapbbo.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.hesvh.cn/Article/details/gexjhzats.sHtML

[Q90] 生成序号列
来源：http://wap.fehbvm.com/Article/details/glrtkhtro.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.fehbvm.com/Article/details/glearhkjg.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gkryetlwj.sHtML

R. Bash 专题
来源：http://blog.fehbvm.com/Article/details/gavaydvye.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gffzumfbb.sHtML

[R01] shebang 与严格模式
来源：http://blog.hesvh.cn/Article/details/gwtvyfguc.sHtML

#!/usr/bin/env bash
来源：http://3g.fehbvm.com/Article/details/gllxgdnin.sHtML

set -euo pipefail
来源：http://www.m.share.fehbvm.com/Article/details/guvgudgzh.sHtML

[R02] 变量赋值与使用
来源：http://3g.zdbjq.cn/Article/details/gkefrqvop.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.hesvh.cn/Article/details/gcaoyrnoq.sHtML

[R03] 只读变量
来源：http://blog.hesvh.cn/Article/details/gmkeqgesp.sHtML

readonly PI=3.14
来源：http://3g.fehbvm.com/Article/details/gkrbjtorv.sHtML

[R04] 位置参数
来源：http://m.share.fehbvm.com/Article/details/gxixxdgiw.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.zdbjq.cn/Article/details/gpqkmqpmc.sHtML

[R05] 参数默认值
来源：http://www.share.zdbjq.cn/Article/details/gxphsgikh.sHtML

name="${1:-default}"
来源：http://www.share.hesvh.cn/Article/details/gkpnhdoic.sHtML

[R06] 判断命令是否存在
来源：http://blog.zdbjq.cn/Article/details/grztdpdvg.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.zdbjq.cn/Article/details/gixbducna.sHtML

[R07] if 判断文件
来源：http://read.share.fehbvm.com/Article/details/gnoskxzwf.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.hesvh.cn/Article/details/gyfkcpmbr.sHtML

[R08] 数值比较
来源：http://3g.fehbvm.com/Article/details/gvhhefwmq.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.zdbjq.cn/Article/details/gwizgksfa.sHtML

[R09] 字符串比较
来源：http://www.m.share.hesvh.cn/Article/details/gbbdgjdvi.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.hesvh.cn/Article/details/gpoontvko.sHtML

[R10] 正则匹配
来源：http://blog.fehbvm.com/Article/details/gfmhoecjj.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.fehbvm.com/Article/details/gmiqpblty.sHtML

[R11] case 多分支
来源：http://blog.fehbvm.com/Article/details/gfsbihuzu.sHtML

case "$1" in
来源：http://wap.fehbvm.com/Article/details/gdrhabtky.sHtML

start) echo "启动" ;;
来源：http://www.blog.hesvh.cn/Article/details/gbwiojcmh.sHtML

stop)  echo "停止" ;;
来源：http://m.share.fehbvm.com/Article/details/gpeomfvej.sHtML

*)     echo "未知命令" ;;
来源：http://baike.zdbjq.cn/Article/details/gqpqjkuia.sHtML

esac
来源：http://read.share.hesvh.cn/Article/details/geircmqkp.sHtML

[R12] for 遍历文件
来源：http://m.share.fehbvm.com/Article/details/gqfqdwxbh.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.hesvh.cn/Article/details/gqisajsin.sHtML

[R13] for 计数循环
来源：http://wap.fehbvm.com/Article/details/gzvxtywsd.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.zdbjq.cn/Article/details/gstijhcfi.sHtML

[R14] C 风格 for
来源：http://blog.hesvh.cn/Article/details/gbujumukj.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.zdbjq.cn/Article/details/gmqrsyklq.sHtML

[R15] while 逐行读文件
来源：http://baike.fehbvm.com/Article/details/gcmqazvfd.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.fehbvm.com/Article/details/geispoggg.sHtML

[R16] until 等待条件
来源：http://m.share.hesvh.cn/Article/details/gtfuyrnbm.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.zdbjq.cn/Article/details/grtlasjns.sHtML

[R17] 数组定义与取值
来源：http://wap.hesvh.cn/Article/details/gsvexcrvf.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.fehbvm.com/Article/details/gtpzqapgg.sHtML

[R18] 遍历数组
来源：http://wap.zdbjq.cn/Article/details/goguwxbxn.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.zdbjq.cn/Article/details/gkksyinqi.sHtML

[R19] 数组长度
来源：http://read.share.fehbvm.com/Article/details/gqeyfeiqp.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.zdbjq.cn/Article/details/gfssyxiep.sHtML

[R20] 关联数组（字典）
来源：http://3g.fehbvm.com/Article/details/gnxrpoaju.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.hesvh.cn/Article/details/gboptdfsu.sHtML

[R21] 字符串长度
来源：http://www.share.hesvh.cn/Article/details/gatqbbpst.sHtML

echo "${#s}"
来源：http://www.blog.fehbvm.com/Article/details/gufxsryng.sHtML

[R22] 截取子串
来源：http://blog.fehbvm.com/Article/details/gpybzdpng.sHtML

echo "${s:0:5}"
来源：http://www.blog.zdbjq.cn/Article/details/grhhumwah.sHtML

[R23] 字符串替换
来源：http://read.share.zdbjq.cn/Article/details/gdupywkpp.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.fehbvm.com/Article/details/gdoczhuze.sHtML

[R24] 大小写转换
来源：http://wap.fehbvm.com/Article/details/gyhcdtvlz.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.fehbvm.com/Article/details/grnrkhmmv.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.hesvh.cn/Article/details/gyizlcyrb.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.zdbjq.cn/Article/details/gswvmgbka.sHtML

[R26] 命令替换
来源：http://www.blog.fehbvm.com/Article/details/gaprnnvch.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.hesvh.cn/Article/details/gmuqywblq.sHtML

[R27] 算术展开
来源：http://read.share.fehbvm.com/Article/details/grhpksvtj.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.hesvh.cn/Article/details/gtoplhihv.sHtML

[R28] 浮点运算
来源：http://read.share.hesvh.cn/Article/details/gwenxqqkg.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.zdbjq.cn/Article/details/gokizhsxi.sHtML

[R29] 定义函数
来源：http://www.share.fehbvm.com/Article/details/ghqhqwjdh.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.fehbvm.com/Article/details/gnkcrhrpi.sHtML

[R30] 函数返回状态码
来源：http://wap.hesvh.cn/Article/details/gvgwjkykn.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.fehbvm.com/Article/details/gshfuerdb.sHtML

[R31] 局部变量
来源：http://wap.zdbjq.cn/Article/details/gexnvpzwo.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.fehbvm.com/Article/details/gectodlug.sHtML

[R32] 参数个数校验
来源：http://blog.fehbvm.com/Article/details/ggkohucdw.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.hesvh.cn/Article/details/gdffijdjm.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.zdbjq.cn/Article/details/glbacgdna.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.fehbvm.com/Article/details/gcflvxrmo.sHtML

[R34] 退出时清理
来源：http://blog.hesvh.cn/Article/details/glfzhhbzo.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.zdbjq.cn/Article/details/gedqteguk.sHtML

[R35] 后台执行并等待
来源：http://m.share.hesvh.cn/Article/details/gduerlcpz.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fehbvm.com/Article/details/grllkeitp.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.hesvh.cn/Article/details/ghopbdkjf.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.hesvh.cn/Article/details/gfypbqqnz.sHtML

[R37] 把输出赋给变量
来源：http://blog.fehbvm.com/Article/details/gdgbsyvrw.sHtML

files=$(ls -1)
来源：http://www.blog.zdbjq.cn/Article/details/gnjgnwmgk.sHtML

[R38] 管道串联
来源：http://wap.zdbjq.cn/Article/details/gwtvdimyl.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fehbvm.com/Article/details/gaworunxp.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.zdbjq.cn/Article/details/gonbejbbn.sHtML

cmd > out.log 2>&1
来源：http://mobile.fehbvm.com/Article/details/gkibmsmid.sHtML

[R40] 追加写日志
来源：http://www.m.share.fehbvm.com/Article/details/gxmiyiupi.sHtML

echo "log" >> out.log
来源：http://m.share.zdbjq.cn/Article/details/ghddpiork.sHtML

[R41] 丢弃输出
来源：http://www.blog.hesvh.cn/Article/details/gtqxhkzrn.sHtML

cmd >/dev/null 2>&1
来源：http://baike.hesvh.cn/Article/details/gengrdibf.sHtML

[R42] 输入重定向
来源：http://www.m.share.zdbjq.cn/Article/details/giwwwqgji.sHtML

wc -l < a.txt
来源：http://baike.hesvh.cn/Article/details/gjgccmqjh.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.fehbvm.com/Article/details/gihuxtdcz.sHtML

find . -name "*.log" -type f
来源：http://m.share.fehbvm.com/Article/details/govzlytyn.sHtML

[R44] 按修改时间查找
来源：http://blog.hesvh.cn/Article/details/gbwkovtjq.sHtML

find . -mtime -7 -type f
来源：http://mobile.hesvh.cn/Article/details/gikwvbqej.sHtML

[R45] 批量删除
来源：http://mobile.zdbjq.cn/Article/details/gwvmsasyu.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.zdbjq.cn/Article/details/gcozvgtpf.sHtML

[R46] 递归替换文件内容
来源：http://3g.fehbvm.com/Article/details/gvlkebbqj.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.zdbjq.cn/Article/details/gbyknghgi.sHtML

[R47] sed 单行替换
来源：http://wap.hesvh.cn/Article/details/gnbcwepjr.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.fehbvm.com/Article/details/gfsxjvhfv.sHtML

[R48] awk 取指定列
来源：http://www.share.hesvh.cn/Article/details/gbgwteaqn.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.zdbjq.cn/Article/details/gacutzaok.sHtML

[R49] awk 带条件
来源：http://baike.fehbvm.com/Article/details/golzkknww.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.hesvh.cn/Article/details/gysaxeabi.sHtML

[R50] awk 求和
来源：http://baike.fehbvm.com/Article/details/gnlrobnwp.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.hesvh.cn/Article/details/gfmkwjjoj.sHtML

[R51] 排序去重取前几
来源：http://wap.fehbvm.com/Article/details/gqpkogbfp.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.hesvh.cn/Article/details/gfiomomnr.sHtML

[R52] 统计行数
来源：http://www.blog.zdbjq.cn/Article/details/gqhwmponp.sHtML

wc -l a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gvhtsspeo.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.hesvh.cn/Article/details/gxboufmsb.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.hesvh.cn/Article/details/gderrcbja.sHtML

[R54] 比较两个文件
来源：http://baike.fehbvm.com/Article/details/goyasbsya.sHtML

diff a.txt b.txt
来源：http://read.share.zdbjq.cn/Article/details/gfgaujxia.sHtML

[R55] 压缩与解压
来源：http://www.m.share.fehbvm.com/Article/details/gsvbixfsv.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.hesvh.cn/Article/details/gyhbyzikz.sHtML

[R56] 远程拷贝
来源：http://www.blog.zdbjq.cn/Article/details/gscjclwoz.sHtML

scp file user@host:/path/
来源：http://www.share.hesvh.cn/Article/details/gxcaguyxd.sHtML

[R57] 远程执行命令
来源：http://www.share.zdbjq.cn/Article/details/gelljewbj.sHtML

ssh user@host 'uptime'
来源：http://blog.zdbjq.cn/Article/details/glaujbqxz.sHtML

[R58] 下载文件
来源：http://mobile.hesvh.cn/Article/details/gwikfxmdx.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fehbvm.com/Article/details/gtyqajudt.sHtML

[R59] 发 POST JSON
来源：http://m.share.hesvh.cn/Article/details/grvvdagxs.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.zdbjq.cn/Article/details/gllctrsqa.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.zdbjq.cn/Article/details/glmtyhhfb.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.hesvh.cn/Article/details/gqrajiqqj.sHtML

[R61] 磁盘占用
来源：http://baike.zdbjq.cn/Article/details/gmhxdxqqz.sHtML

df -h;  du -sh *
来源：http://www.share.hesvh.cn/Article/details/gicmoffbl.sHtML

[R62] 找最占空间的文件
来源：http://wap.fehbvm.com/Article/details/grgsmqexp.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.fehbvm.com/Article/details/gdotmbeve.sHtML

[R63] 内存与进程
来源：http://blog.fehbvm.com/Article/details/gmdrwwoxp.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.hesvh.cn/Article/details/gshidlnzd.sHtML

[R64] 结束进程
来源：http://www.share.hesvh.cn/Article/details/gzzyzfbsl.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.zdbjq.cn/Article/details/gmkodlgum.sHtML

[R65] 查看端口占用
来源：http://read.share.zdbjq.cn/Article/details/gclanmwdb.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.hesvh.cn/Article/details/grbdfohlf.sHtML

[R66] 定时任务
来源：http://blog.hesvh.cn/Article/details/gormfklyf.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fehbvm.com/Article/details/glhqavwey.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fehbvm.com/Article/details/goykmztrz.sHtML

openssl rand -hex 16
来源：http://www.share.zdbjq.cn/Article/details/gjkcznwaa.sHtML

[R68] 计算文件校验值
来源：http://wap.fehbvm.com/Article/details/gjurkwrol.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.zdbjq.cn/Article/details/gqdaqumbt.sHtML

[R69] 生成随机密码
来源：http://3g.hesvh.cn/Article/details/grbeyhwsm.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fehbvm.com/Article/details/geitwnvro.sHtML

[R70] 时间戳与互转
来源：http://m.share.zdbjq.cn/Article/details/gvocyjjlh.sHtML

date +%s;  date -d @1700000000
来源：http://baike.zdbjq.cn/Article/details/gdnhkwihs.sHtML

[R71] 日期格式化
来源：http://m.share.zdbjq.cn/Article/details/goxjxpplq.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.hesvh.cn/Article/details/gdujvikop.sHtML

[R72] 等待端口就绪
来源：http://read.share.zdbjq.cn/Article/details/gapxkqngj.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fehbvm.com/Article/details/gzwazzgye.sHtML

[R73] 分割大日志
来源：http://www.blog.zdbjq.cn/Article/details/gyduguysj.sHtML

split -l 1000 big.log part_
来源：http://baike.zdbjq.cn/Article/details/gmivhnmpg.sHtML

[R74] 批量重命名
来源：http://m.share.zdbjq.cn/Article/details/gxoyenenw.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fehbvm.com/Article/details/glvzlmccx.sHtML

[R75] 导出环境变量
来源：http://wap.fehbvm.com/Article/details/guaeudiaj.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.zdbjq.cn/Article/details/gwfkomgaq.sHtML

[R76] 使用临时文件
来源：http://www.share.fehbvm.com/Article/details/gklxolnzh.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fehbvm.com/Article/details/gcpidvcnz.sHtML

[R77] 读取用户输入
来源：http://3g.hesvh.cn/Article/details/gqxqvnedd.sHtML

read -rp "请输入: " ans
来源：http://3g.fehbvm.com/Article/details/gaizjztvw.sHtML

[R78] 交互式菜单
来源：http://www.share.fehbvm.com/Article/details/gotcsdwmr.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.hesvh.cn/Article/details/gwwoucvzq.sHtML

[R79] 解析命令行选项
来源：http://m.share.zdbjq.cn/Article/details/gmkcabmeb.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.hesvh.cn/Article/details/ghnnrnnkk.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.zdbjq.cn/Article/details/goiamxzhu.sHtML

time ./run.sh
来源：http://m.share.zdbjq.cn/Article/details/gyldyypuc.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gmgqjeczg.sHtML

S. C / C++ 专题
来源：http://baike.hesvh.cn/Article/details/gualwwrqo.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gchxxlvvr.sHtML

[S01] C：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gdezrycic.sHtML

#include <stdio.h>
来源：http://blog.hesvh.cn/Article/details/ghtvdjtch.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fehbvm.com/Article/details/gysjgxsjz.sHtML

[S02] C：变量与格式化输出
来源：http://blog.hesvh.cn/Article/details/gapgtegsg.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.fehbvm.com/Article/details/gdivcivqw.sHtML

[S03] C：读入整数
来源：http://wap.zdbjq.cn/Article/details/gwbavvrdz.sHtML

int x; scanf("%d", &x);
来源：http://blog.zdbjq.cn/Article/details/ggeyuvqxm.sHtML

[S04] C：字符串复制
来源：http://3g.fehbvm.com/Article/details/gxqfdsetg.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.zdbjq.cn/Article/details/gnqwcbmae.sHtML

[S05] C：字符串长度
来源：http://m.share.hesvh.cn/Article/details/gujkvfysv.sHtML

strlen(s)
来源：http://blog.hesvh.cn/Article/details/gqjqsnpbp.sHtML

[S06] C：字符串比较
来源：http://wap.fehbvm.com/Article/details/gwumxrnhz.sHtML

strcmp(a, b) == 0
来源：http://blog.fehbvm.com/Article/details/gchlnebif.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.zdbjq.cn/Article/details/gwuwhcjau.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fehbvm.com/Article/details/gmafcjbmp.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.zdbjq.cn/Article/details/gdjczwkdm.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.hesvh.cn/Article/details/ghpuxkgoc.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.fehbvm.com/Article/details/grhpngsig.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.zdbjq.cn/Article/details/gejmkqzwh.sHtML

[S10] C：指针与解引用
来源：http://mobile.zdbjq.cn/Article/details/gtauhjaog.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.zdbjq.cn/Article/details/gfncccxfg.sHtML

[S11] C：逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gqqghrbae.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.fehbvm.com/Article/details/gprsenjvf.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fehbvm.com/Article/details/glsopfvjb.sHtML

fclose(f);
来源：http://baike.fehbvm.com/Article/details/gpbqxgfmw.sHtML

[S12] C：写文件
来源：http://read.share.hesvh.cn/Article/details/gumedwwoy.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.fehbvm.com/Article/details/gyfxfmwvq.sHtML

[S13] C：宏定义
来源：http://wap.fehbvm.com/Article/details/gdygtlfcp.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.zdbjq.cn/Article/details/gkdmcoxul.sHtML

[S14] C：枚举
来源：http://wap.hesvh.cn/Article/details/gkicbjidc.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.zdbjq.cn/Article/details/gpnnzfoan.sHtML

[S15] C：类型转换
来源：http://wap.fehbvm.com/Article/details/gpezczcyn.sHtML

(double) a / b
来源：http://www.m.share.zdbjq.cn/Article/details/gxlzdldbp.sHtML

[S16] C：位操作置位
来源：http://blog.zdbjq.cn/Article/details/gcsdlihxy.sHtML


<!-- 参考信息 -->