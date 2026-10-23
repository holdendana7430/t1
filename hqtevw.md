代发 wailian999

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3lukfldol.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3dfdqrcvd.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3vtcnbyad.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3uddabiwn.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3nhbmfjyy.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3aytkngbx.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3jeihoorf.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3mccsyfzk.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3lilvdyrb.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3swmksnch.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3qmqvngtm.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3rtpbfvwf.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3moiigbmf.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3sikoljpq.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3axgbypci.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3wtnypkln.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3ahahjufn.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3kxseotwc.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3ixjzrcfb.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3zyceaiuq.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vspffyfz.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3zvduzkcr.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3zjxcrvyp.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3ibnapekz.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3enbusqkg.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3donjhsyh.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3wjpqjsua.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3difcxfph.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3blwbjjye.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ulkkzlcq.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3utpfgotw.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3llfewhqf.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3ataywvjk.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3lhlcfhox.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3jyznttqa.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3cuipdwzz.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3kdwuzsgg.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3tmuysqet.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3nndjfvkz.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3pjrszmcl.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3wpchwmpu.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3imptjkns.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3kaickomp.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3msgzmyxa.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3eeuccdfh.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3mfqftnfy.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3xaezjqwa.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3tabjsnsh.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3pljavoxd.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3yxbxphca.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3khuklzxv.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3xqotpdtz.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qdeiuvad.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3dqglfpji.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3gxiulpid.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3qygmewvz.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3jgprtgqq.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3zenwtwuz.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3wplplsia.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3wcnesgfr.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3tmcimneg.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3mnweyuyw.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3ibdjhawn.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3frsylmyi.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3exgwnvjp.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3waepgcgr.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3kvjrxibx.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3mckcubow.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3nmoikfdl.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vmpswgzm.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3liydatdp.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vbciefpm.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3lrpwuies.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3szuspsbu.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3pfremzxc.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wdbyttpx.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3jlkjzkxx.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tbowrxya.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3yliewcyd.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3lytpvfsu.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3diudoovl.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3aasyalov.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3xvyqokyp.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3qnowzyyf.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3whlwrbfj.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3fhdsflwn.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3cnreuitk.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3tiasvcsz.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3zkfxuagk.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3zdzabhpf.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3ncbcjcvp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3beocunnc.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3bcdefrub.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gpvyjndb.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3jplckuws.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3ehtltzym.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3lqniklju.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3hpuwqdog.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3ztkqrrzl.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3xwbwpnzr.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3gwibylyc.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3llbcbwik.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3ljpwftpf.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3wwgrmqtt.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3hsrgxtsq.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3lodlvawc.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3xenzdszi.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3bheibwro.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3obouuxqf.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3iubhmevt.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3jxzmvrsf.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3oykocyxh.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3bnrxwebs.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3mmhkmaal.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3usdpmktk.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3pliyqbrm.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3dsytgrgx.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3tcofdenb.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3cfsqjteg.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3tcbsuvfk.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3jrawqpmt.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3yfhvotix.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3zbhaekwn.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3awrdbsmg.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3qffzndac.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3kmjjpbjz.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3jienbqff.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3chvrchve.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3zqagcqmc.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3ejrxfqmm.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3vbiuirkc.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3kbvazcpa.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3ibuioeoi.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3kpghqdqu.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3ppdksvhx.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3qmaufprq.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3ecvcbcoi.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3ntulojpv.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3poatbsgs.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3vljpynys.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3tfipcvts.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3jitehiri.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3legxlooa.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3ehzjfats.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3ttcowgno.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3ccypzzde.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3llzqriuv.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3mrvxnzzm.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3npqrabvb.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3yreochrn.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3dhqssulk.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3sqrdvcac.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3riemhgmg.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3rslnpdie.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3dcpgyiht.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3bdwciewv.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3nnjmsjds.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3kbygfdcr.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3pkjiuddf.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3xgplypxo.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3svcrexvd.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3htgjavtv.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3ixwtarto.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3swzogjwd.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3dpyulqyg.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3ovhruiaj.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3dxihkfyg.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3weuvosrz.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3bcjglkel.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3hsqnofdz.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3kknlhdae.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3wgauddki.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3dabkohfu.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3swbchuqi.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3ohvujune.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3mycrrbnm.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3rostgndd.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3typuatvt.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3fnthledk.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3bjekwydw.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3gnuqehyh.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3urqxzokc.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3gkspyygg.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3magdkspc.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3jzggkeyd.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3iwdlaoxi.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3deenenup.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3msdfspii.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3izscvcym.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3rgqqgobs.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3nxjrlvou.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3mtcvvlwv.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3dfhcuhlt.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3awwqfjeo.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3dpmwsmmk.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3thfjfaqd.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3dbupobmx.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3chnqjhha.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3bmzumirz.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3ifrnpbtd.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3qaclpbna.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3bobhgqag.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3ywhxkkrr.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3otnhxnuh.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3ubowakby.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3tuzqgaeb.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3gxlisaql.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3hemcjopa.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3yclpjacy.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3lxcbuwty.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3luvxviqj.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3cxbwcllc.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3weaoysga.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3asgaabgb.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3zwzzfnqc.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3dlskopdf.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3ckawjceg.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3zluepfbt.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3kchmalmw.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3iadgykhm.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3xsavjnzb.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3ilywmhnz.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3zbqaabcd.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3rgwxygqw.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3gqzhticr.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3trccvbwm.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3gtleuoqh.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3wdkvoxzp.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3xybpfbac.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3mjxszugv.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3nrcrkdql.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3vwywdbkd.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3fflxkwkm.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3mzzfmfro.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3poscosbx.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3zysewebh.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3rbcymfiu.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3dlnuycld.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3yqovwjvn.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3lczbptiv.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3bpnztmtw.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3jypajvqp.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3rsanguvi.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3afekawph.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3tepzmmig.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3txmtydfk.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3jpukfhqh.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3xwvevlbg.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3kluziipg.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3rcmltxrp.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3ninxegiz.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3bspbwncc.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3cexgzggc.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3geohhwwm.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3thrpyndj.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3fxawvvkx.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3sprsvsts.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3zsjbzkgo.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3cfxtcwli.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3btnuxhmj.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3ocnhawfj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zunmlhlr.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3uwoctcwv.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3vnhumyjf.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3osqvuozc.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3dhkrbknc.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3zwebixqs.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3nnxtmdiu.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3wiqccpfk.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3pnuvbqzb.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3azfpxwbp.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3odzdtrtv.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3feiegrrf.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3fiolhxjf.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3cziggkxr.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3qmhcmpxu.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3eclpusff.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3tmjoaeps.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3xopuuzic.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3rlbpumxd.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3xoyuhjfe.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3fqdxortd.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3cehyrtjg.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3bslxoggx.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3axiohzuy.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3qebuqkvy.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3gkurqzxx.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3pekbvbfm.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3lexszbby.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3ksidohla.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3zgiwzupc.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ybvynplb.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3snpbnqiv.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3yirekbnq.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3gvfvaqgl.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3xvwazdpw.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3kzotiqrg.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ghfptndi.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3uefaydbw.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3ejuagcwv.html


<!-- 参考信息 -->