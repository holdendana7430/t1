代发 wailian999

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsevxswqr.sHtML

[Q52] 删除指定行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsyldrpyt.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmqjfxoon.sHtML

[Q53] 按条件删除
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqzenmjvc.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.fanxiaobao.xyz/Article/details/griqmdafc.sHtML

[Q54] 清空表
来源：http://wap.fanxiaobao.xyz/Article/details/gxvwdywxx.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.fanxiaobao.xyz/Article/details/gwftityln.sHtML

[Q55] 排名（并列占位）
来源：http://blog.fanxiaobao.xyz/Article/details/gyaewzfxy.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmwpasfvm.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.fanxiaobao.xyz/Article/details/gtfohujbc.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.fanxiaobao.xyz/Article/details/gasmutymg.sHtML

[Q57] 行号
来源：http://m.share.fanxiaobao.xyz/Article/details/grwkiabxl.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gcrlnuffi.sHtML

[Q58] 累计求和
来源：http://baike.fanxiaobao.xyz/Article/details/ghpuqbalv.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/govbyfvne.sHtML

[Q59] 分组内累计
来源：http://blog.fanxiaobao.xyz/Article/details/gpbdpgfzk.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gstvydcrm.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.fanxiaobao.xyz/Article/details/gjftxjpgj.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.fanxiaobao.xyz/Article/details/gruwrixli.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gzxxxvuve.sHtML

[Q61] 移动平均
来源：http://mobile.fanxiaobao.xyz/Article/details/gcrpaxvsq.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghyowugqo.sHtML

[Q62] 分组占比
来源：http://mobile.fanxiaobao.xyz/Article/details/gjcewjity.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkzdndbrj.sHtML

[Q63] 开启事务
来源：http://mobile.fanxiaobao.xyz/Article/details/gykpzykvj.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.fanxiaobao.xyz/Article/details/gebvtgqyo.sHtML

[Q64] 提交事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gftnshldd.sHtML

COMMIT;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjdbdtxzc.sHtML

[Q65] 回滚事务
来源：http://read.share.fanxiaobao.xyz/Article/details/gtvpuxtpw.sHtML

ROLLBACK;
来源：http://www.share.fanxiaobao.xyz/Article/details/gqdlkmsus.sHtML

[Q66] 行锁查询
来源：http://mobile.fanxiaobao.xyz/Article/details/gwbeqrqzs.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.fanxiaobao.xyz/Article/details/ggvarwjpb.sHtML

[Q67] 设置隔离级别
来源：http://www.share.fanxiaobao.xyz/Article/details/gpztwwjwz.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.fanxiaobao.xyz/Article/details/gxdmynypx.sHtML

[Q68] 保存点
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glptdjvhq.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggsqyzlpt.sHtML

ROLLBACK TO sp1;
来源：http://baike.fanxiaobao.xyz/Article/details/gtfaeozvh.sHtML

[Q69] 查看执行计划
来源：http://3g.fanxiaobao.xyz/Article/details/grjyigfgc.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.fanxiaobao.xyz/Article/details/gjdgpjuaq.sHtML

[Q70] 更新统计信息
来源：http://3g.fanxiaobao.xyz/Article/details/gdgzruurx.sHtML

ANALYZE TABLE users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gmyqkdejg.sHtML

[Q71] 查看建表语句
来源：http://baike.fanxiaobao.xyz/Article/details/ghjatwtuv.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.fanxiaobao.xyz/Article/details/gstdjficn.sHtML

[Q72] 查看索引
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grogtseaw.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/geycriucx.sHtML

[Q73] 查看表状态
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggrsuebvj.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfrbiufld.sHtML

[Q74] 强制使用索引
来源：http://3g.fanxiaobao.xyz/Article/details/gmudjawxq.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.fanxiaobao.xyz/Article/details/gximitvvz.sHtML

[Q75] 日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gswzcjcxd.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gomjhshum.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.fanxiaobao.xyz/Article/details/gnrwnxnvt.sHtML

[Q76] 按天统计
来源：http://wap.fanxiaobao.xyz/Article/details/gxintwoli.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.fanxiaobao.xyz/Article/details/gnzcodwmh.sHtML

[Q77] 时间加减
来源：http://www.share.fanxiaobao.xyz/Article/details/gacgnyafh.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.fanxiaobao.xyz/Article/details/guvguvrcw.sHtML

[Q78] 当前时间
来源：http://m.share.fanxiaobao.xyz/Article/details/gmjjslamm.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwvlsugep.sHtML

[Q79] 字符串拼接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcgrbrvex.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.fanxiaobao.xyz/Article/details/gmazxrupm.sHtML

[Q80] 字符串截取
来源：http://wap.fanxiaobao.xyz/Article/details/gwadvejon.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/ghedffier.sHtML

[Q81] 字符串替换
来源：http://3g.fanxiaobao.xyz/Article/details/glkqgjhun.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gxqhwykxj.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.fanxiaobao.xyz/Article/details/glulniaus.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gogfswdix.sHtML

[Q83] 大小写转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gxblmutfg.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdhxglspb.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnuvkasvj.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gcxfvexwt.sHtML

[Q85] 数值取整
来源：http://3g.fanxiaobao.xyz/Article/details/gfplomnvx.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.fanxiaobao.xyz/Article/details/gkdldknfl.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.fanxiaobao.xyz/Article/details/gvdvocssx.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.fanxiaobao.xyz/Article/details/gwzuxbvxg.sHtML

[Q87] JSON 字段做条件
来源：http://baike.fanxiaobao.xyz/Article/details/gnwupdbff.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.fanxiaobao.xyz/Article/details/grnmmdobg.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.fanxiaobao.xyz/Article/details/gsilyirsm.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glkjfpiaj.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gbfewlfvu.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfpatoiiu.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.fanxiaobao.xyz/Article/details/gjvclzffn.sHtML

[Q90] 生成序号列
来源：http://baike.fanxiaobao.xyz/Article/details/gizxnmcbj.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.fanxiaobao.xyz/Article/details/gmnljaxht.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/giujdnfhl.sHtML

R. Bash 专题
来源：http://blog.fanxiaobao.xyz/Article/details/gttezkhdf.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gmieqapkw.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkfvlgsbq.sHtML

#!/usr/bin/env bash
来源：http://read.share.fanxiaobao.xyz/Article/details/gvvltcfol.sHtML

set -euo pipefail
来源：http://read.share.fanxiaobao.xyz/Article/details/gjwyzkggk.sHtML

[R02] 变量赋值与使用
来源：http://3g.fanxiaobao.xyz/Article/details/gaaxnpulj.sHtML

name="Tom"; echo "$name"
来源：http://mobile.fanxiaobao.xyz/Article/details/gnemekzbz.sHtML

[R03] 只读变量
来源：http://wap.fanxiaobao.xyz/Article/details/gkxbynzzr.sHtML

readonly PI=3.14
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnvtrlwhf.sHtML

[R04] 位置参数
来源：http://3g.fanxiaobao.xyz/Article/details/gsqlqlmit.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.fanxiaobao.xyz/Article/details/giczjuwjd.sHtML

[R05] 参数默认值
来源：http://m.share.fanxiaobao.xyz/Article/details/gaxgygqqc.sHtML

name="${1:-default}"
来源：http://blog.fanxiaobao.xyz/Article/details/gbcxojvwa.sHtML

[R06] 判断命令是否存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gfdqpfdxe.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gleivunbf.sHtML

[R07] if 判断文件
来源：http://wap.fanxiaobao.xyz/Article/details/gtrsjhynt.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gbcwcrcdo.sHtML

[R08] 数值比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gstlonyvx.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gwlgopvfx.sHtML

[R09] 字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gwjgpxpmb.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqtezmlza.sHtML

[R10] 正则匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjbkqddfs.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gibfsrtne.sHtML

[R11] case 多分支
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsrmgttfv.sHtML

case "$1" in
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzipmdygc.sHtML

start) echo "启动" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmmyeyuhq.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gywwqmvwp.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/gehxapehh.sHtML

esac
来源：http://blog.fanxiaobao.xyz/Article/details/guzsaxehg.sHtML

[R12] for 遍历文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gffnsiukl.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gpxxbidly.sHtML

[R13] for 计数循环
来源：http://www.share.fanxiaobao.xyz/Article/details/geqoooiuf.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gsinjgjgb.sHtML

[R14] C 风格 for
来源：http://read.share.fanxiaobao.xyz/Article/details/gndcycdea.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gqreljaun.sHtML

[R15] while 逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gbfxqoven.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmclvnlai.sHtML

[R16] until 等待条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsyazihhe.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/gudokvddh.sHtML

[R17] 数组定义与取值
来源：http://read.share.fanxiaobao.xyz/Article/details/gyopyjwll.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gixsuydqz.sHtML

[R18] 遍历数组
来源：http://wap.fanxiaobao.xyz/Article/details/gbxseados.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gajdndhau.sHtML

[R19] 数组长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gavzdkhxk.sHtML

echo "${#arr[@]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gypdxfdua.sHtML

[R20] 关联数组（字典）
来源：http://blog.fanxiaobao.xyz/Article/details/getkpstrq.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gqfyhzxke.sHtML

[R21] 字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/gejiyrrxe.sHtML

echo "${#s}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gpgtyaatb.sHtML

[R22] 截取子串
来源：http://www.share.fanxiaobao.xyz/Article/details/gonxfwlaj.sHtML

echo "${s:0:5}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gdyyplkqz.sHtML

[R23] 字符串替换
来源：http://wap.fanxiaobao.xyz/Article/details/gnnqyemii.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbdwhyrxj.sHtML

[R24] 大小写转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/guytgjohk.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.fanxiaobao.xyz/Article/details/gyfhvzjnt.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.fanxiaobao.xyz/Article/details/gtdijjivk.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fanxiaobao.xyz/Article/details/guegggjeb.sHtML

[R26] 命令替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grqmubykk.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsiksywnl.sHtML

[R27] 算术展开
来源：http://wap.fanxiaobao.xyz/Article/details/gmzpegkrm.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsiulngsw.sHtML

[R28] 浮点运算
来源：http://wap.fanxiaobao.xyz/Article/details/gcgkvewjh.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.fanxiaobao.xyz/Article/details/gmtifeuci.sHtML

[R29] 定义函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gwflfpcdi.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyqjywvnn.sHtML

[R30] 函数返回状态码
来源：http://read.share.fanxiaobao.xyz/Article/details/gobunwjsx.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfihhwitl.sHtML

[R31] 局部变量
来源：http://blog.fanxiaobao.xyz/Article/details/gsiluchwd.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gtgrhazlh.sHtML

[R32] 参数个数校验
来源：http://3g.fanxiaobao.xyz/Article/details/gmgbljstd.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/ghpkyleqi.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fanxiaobao.xyz/Article/details/ggolvcgzc.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.fanxiaobao.xyz/Article/details/gxwrtehti.sHtML

[R34] 退出时清理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbadajrmb.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.fanxiaobao.xyz/Article/details/gcgjeoxmb.sHtML

[R35] 后台执行并等待
来源：http://mobile.fanxiaobao.xyz/Article/details/ggoayuuxg.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fanxiaobao.xyz/Article/details/glugjzckp.sHtML

[R36] 并发执行多个任务
来源：http://3g.fanxiaobao.xyz/Article/details/gtwovbauw.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggvyxenre.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxngpthhe.sHtML

files=$(ls -1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvkgdqmdw.sHtML

[R38] 管道串联
来源：http://blog.fanxiaobao.xyz/Article/details/gvcmlktlj.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/gglfygqqf.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.fanxiaobao.xyz/Article/details/gtflvcthj.sHtML

cmd > out.log 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/gjldtqxjt.sHtML

[R40] 追加写日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gvddngygh.sHtML

echo "log" >> out.log
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grxumqskn.sHtML

[R41] 丢弃输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gfhwpdiev.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.fanxiaobao.xyz/Article/details/gvaexycmu.sHtML

[R42] 输入重定向
来源：http://wap.fanxiaobao.xyz/Article/details/gyyrtoztu.sHtML

wc -l < a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gjddwnsre.sHtML

[R43] 按名字查找文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gaxbyhtfl.sHtML

find . -name "*.log" -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/gobswdwzf.sHtML

[R44] 按修改时间查找
来源：http://baike.fanxiaobao.xyz/Article/details/gmshpkyrl.sHtML

find . -mtime -7 -type f
来源：http://3g.fanxiaobao.xyz/Article/details/gpgnaqkns.sHtML

[R45] 批量删除
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwxyzrged.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.fanxiaobao.xyz/Article/details/gbeqleeem.sHtML

[R46] 递归替换文件内容
来源：http://blog.fanxiaobao.xyz/Article/details/gdtrgvsuc.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.fanxiaobao.xyz/Article/details/gowupbzqp.sHtML

[R47] sed 单行替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdxxyddez.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gpirwqvhu.sHtML

[R48] awk 取指定列
来源：http://3g.fanxiaobao.xyz/Article/details/ghmkbqbbj.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gwbbefyhg.sHtML

[R49] awk 带条件
来源：http://3g.fanxiaobao.xyz/Article/details/gatitcjzd.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fanxiaobao.xyz/Article/details/grjumltan.sHtML

[R50] awk 求和
来源：http://blog.fanxiaobao.xyz/Article/details/gnlamfynf.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gedxrlqdu.sHtML

[R51] 排序去重取前几
来源：http://baike.fanxiaobao.xyz/Article/details/gerlpiorj.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fanxiaobao.xyz/Article/details/gavsuuors.sHtML

[R52] 统计行数
来源：http://m.share.fanxiaobao.xyz/Article/details/gzjqeuwuh.sHtML

wc -l a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gltkbqpdp.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.fanxiaobao.xyz/Article/details/gmgmgfelz.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.fanxiaobao.xyz/Article/details/gnzqtfzpa.sHtML

[R54] 比较两个文件
来源：http://wap.fanxiaobao.xyz/Article/details/gnryjvnou.sHtML

diff a.txt b.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gxbtjioas.sHtML

[R55] 压缩与解压
来源：http://m.share.fanxiaobao.xyz/Article/details/ghikmxgoe.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fanxiaobao.xyz/Article/details/gcoffrqki.sHtML

[R56] 远程拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/gdnjeccwt.sHtML

scp file user@host:/path/
来源：http://3g.fanxiaobao.xyz/Article/details/gyonmddwn.sHtML

[R57] 远程执行命令
来源：http://m.share.fanxiaobao.xyz/Article/details/gppasymnj.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzxqmfkiy.sHtML

[R58] 下载文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gognsqdxl.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fanxiaobao.xyz/Article/details/gnwrzshuj.sHtML

[R59] 发 POST JSON
来源：http://www.blog.fanxiaobao.xyz/Article/details/goxpnsikr.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fanxiaobao.xyz/Article/details/glxcegfkt.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.fanxiaobao.xyz/Article/details/ggqizoytu.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.fanxiaobao.xyz/Article/details/gfedbwtyq.sHtML

[R61] 磁盘占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmawmqfko.sHtML

df -h;  du -sh *
来源：http://mobile.fanxiaobao.xyz/Article/details/gfnrhzrzk.sHtML

[R62] 找最占空间的文件
来源：http://wap.fanxiaobao.xyz/Article/details/gnkkpsyqv.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.fanxiaobao.xyz/Article/details/gkohwbhqv.sHtML

[R63] 内存与进程
来源：http://blog.fanxiaobao.xyz/Article/details/giiasmddt.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.fanxiaobao.xyz/Article/details/gjssabjyb.sHtML

[R64] 结束进程
来源：http://www.share.fanxiaobao.xyz/Article/details/gmhwbiqmd.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvlkblteb.sHtML

[R65] 查看端口占用
来源：http://blog.fanxiaobao.xyz/Article/details/gmdstuawi.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.fanxiaobao.xyz/Article/details/gqymnfkth.sHtML

[R66] 定时任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkcejgkqe.sHtML

crontab -e;  crontab -l
来源：http://read.share.fanxiaobao.xyz/Article/details/gqlczzhbn.sHtML

[R67] 生成随机十六进制串
来源：http://blog.fanxiaobao.xyz/Article/details/gwqkyigsh.sHtML

openssl rand -hex 16
来源：http://m.share.fanxiaobao.xyz/Article/details/gpzwmlrlk.sHtML

[R68] 计算文件校验值
来源：http://blog.fanxiaobao.xyz/Article/details/gfenlvdcb.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gnmgklpfe.sHtML

[R69] 生成随机密码
来源：http://m.share.fanxiaobao.xyz/Article/details/ggyycsnwa.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.fanxiaobao.xyz/Article/details/gomjyrlaj.sHtML

[R70] 时间戳与互转
来源：http://3g.fanxiaobao.xyz/Article/details/gyrbhsnim.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fanxiaobao.xyz/Article/details/gyjxdobkh.sHtML

[R71] 日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/ggaskigfs.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.fanxiaobao.xyz/Article/details/gdiknopml.sHtML

[R72] 等待端口就绪
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxzivvvlt.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfgjhtyav.sHtML

[R73] 分割大日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goiieustu.sHtML

split -l 1000 big.log part_
来源：http://3g.fanxiaobao.xyz/Article/details/gdxpuwpxg.sHtML

[R74] 批量重命名
来源：http://baike.fanxiaobao.xyz/Article/details/grishllvu.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gioyydaga.sHtML

[R75] 导出环境变量
来源：http://wap.fanxiaobao.xyz/Article/details/gkpxuredk.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.fanxiaobao.xyz/Article/details/gnwuprokg.sHtML

[R76] 使用临时文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gburpnpis.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/gmetzratt.sHtML

[R77] 读取用户输入
来源：http://baike.fanxiaobao.xyz/Article/details/gnwgxmxwl.sHtML

read -rp "请输入: " ans
来源：http://baike.fanxiaobao.xyz/Article/details/ggvtiiied.sHtML

[R78] 交互式菜单
来源：http://blog.fanxiaobao.xyz/Article/details/govgikvnb.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.fanxiaobao.xyz/Article/details/ggqeqthmd.sHtML

[R79] 解析命令行选项
来源：http://3g.fanxiaobao.xyz/Article/details/gsphpbrba.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpuponjzq.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fanxiaobao.xyz/Article/details/gtkyqrlbw.sHtML

time ./run.sh
来源：http://blog.fanxiaobao.xyz/Article/details/gaftowedk.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gbjrjupvs.sHtML

S. C / C++ 专题
来源：http://m.share.fanxiaobao.xyz/Article/details/gotvwyake.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gltxqgops.sHtML

[S01] C：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbjtzkkxm.sHtML

#include <stdio.h>
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmfjxvalv.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmqyepgcf.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/glqcgqijr.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.fanxiaobao.xyz/Article/details/gankgazcd.sHtML

[S03] C：读入整数
来源：http://blog.fanxiaobao.xyz/Article/details/gklfmsphq.sHtML

int x; scanf("%d", &x);
来源：http://mobile.fanxiaobao.xyz/Article/details/gggbtgrlo.sHtML

[S04] C：字符串复制
来源：http://www.blog.fanxiaobao.xyz/Article/details/giabcmwnn.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.fanxiaobao.xyz/Article/details/gxrllfucp.sHtML

[S05] C：字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gfimsmzcw.sHtML

strlen(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gagyqpohz.sHtML

[S06] C：字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/guyndpoch.sHtML

strcmp(a, b) == 0
来源：http://blog.fanxiaobao.xyz/Article/details/gusgdaxsk.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gqfeaduyj.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbnqslfts.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fanxiaobao.xyz/Article/details/gzfalnkfk.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.fanxiaobao.xyz/Article/details/groodhcfd.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.fanxiaobao.xyz/Article/details/gohldqsdt.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fanxiaobao.xyz/Article/details/goittjsri.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzqijckhh.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fanxiaobao.xyz/Article/details/gsshvrfqe.sHtML

[S11] C：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gdspnwcbf.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmfahctke.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvzmgpvls.sHtML

fclose(f);
来源：http://mobile.fanxiaobao.xyz/Article/details/gytgepwoy.sHtML

[S12] C：写文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghhronpkl.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwwarggip.sHtML

[S13] C：宏定义
来源：http://mobile.fanxiaobao.xyz/Article/details/gocexegpr.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fanxiaobao.xyz/Article/details/gisejbwyj.sHtML

[S14] C：枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/gonjtnbrp.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsaiyvjry.sHtML

[S15] C：类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gtshfjqaa.sHtML

(double) a / b
来源：http://mobile.fanxiaobao.xyz/Article/details/gdrgikxmq.sHtML

[S16] C：位操作置位
来源：http://read.share.fanxiaobao.xyz/Article/details/gjouvhgia.sHtML

x |= (1 << 3);
来源：http://baike.fanxiaobao.xyz/Article/details/ggowuwuqi.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gkwrodfys.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fanxiaobao.xyz/Article/details/gbkkroasv.sHtML

[S18] C：命令行参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gvojzfqwi.sHtML

int main(int argc, char **argv)
来源：http://wap.fanxiaobao.xyz/Article/details/gxmzzmsws.sHtML

[S19] C：快速排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqzkzswap.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/gpdrxkoar.sHtML

[S20] C：二分查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geilpfbmz.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/gyngdpgma.sHtML

[S21] C：字符类别判断
来源：http://3g.fanxiaobao.xyz/Article/details/gybwacuug.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.fanxiaobao.xyz/Article/details/gtigzjcxg.sHtML

[S22] C：字符串转数字
来源：http://mobile.fanxiaobao.xyz/Article/details/gjmmxfoqn.sHtML


<!-- 参考信息 -->