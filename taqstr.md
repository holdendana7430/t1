代发 wailian999

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3kdahlckk.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3qugqqxqj.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3gsfqbubz.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3uarqnadd.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3azzvvajq.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3jxcvrtmf.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3daaqxapd.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3lhxuoxna.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rdqkzsyu.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3ioblfspv.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ybpbfpqv.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3roswxdxq.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3gnpocibb.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3izkpjhsi.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3byypinjq.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3axjvapbq.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3wayynzwy.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ogehmlwv.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3csrcozrj.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3ntbdiljs.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3gorlxvbn.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3fkbzdrtp.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3gysdsvoi.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3sujnhzax.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3lbcabovw.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3nkibvmtp.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3cwpbkjqt.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3zepjrzah.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3caykfrzj.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3jktlkfya.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3maacuwdw.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3bqiiuajd.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3grgbcmwf.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3tmxifque.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3wyqwvdwa.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3xqjnkpzw.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3hqsepjrm.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3uucqobqe.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3yjnswgoe.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3wvvtsbus.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ljgjglpr.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3uoahxgjv.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3mpavojcd.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3blyqdsmr.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3lthhtppo.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3sphjbnzb.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3advvwbbu.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3rxirrlnz.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3xdectmhn.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3zbnkmvuj.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3nydtoero.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3stmiylgh.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3hotopomy.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3lypqadbw.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3twnjxguu.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3bxfwyikp.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3whocmugo.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3upffcdia.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3oudarpyd.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3duoduqnq.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3ttpugnik.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hspdajul.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3duhlzefw.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xyzqyfwc.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3rlqucrwm.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zhbwvtps.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3ggxyinul.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3wsbibojc.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3amaqwtry.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3mzmlrnkk.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3penqwqco.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3ihpesjfa.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3xewioeex.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3kumflkqx.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3phfapufy.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3quwzrjzh.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3dvwwuhdq.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3brlgvpdt.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3wlbvdpgg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3otsnbbbl.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3izaclebh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uiiumoim.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3ggzxlcpy.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3pgxlizvl.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3ntlrekqy.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3nbyzvewp.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3ketarynk.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3lxjddtha.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3wvmpynok.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3fcahtflo.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3gvtkqoxh.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3sfbfviqm.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3fuezxsit.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3oeqllcvl.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3grrwscwt.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3plknskni.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3xxqnqdps.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3sxomlyfm.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3ptmajncz.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3yphxqcog.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3rhsibymc.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3cgmjuosz.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3pzwwbruj.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3ntztywfu.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3ddusitsy.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3zfttmuaz.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3cejoeckb.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3vsfppoaw.html

esac
来源：http://www.52xcode.cn/Article/details/gt3zhqwsvnd.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3qcjmbjns.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3okwgpwaq.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3woetquid.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3cwuacpme.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3ewfhsrya.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3cgmrcfyd.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3lmsfimmt.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3mciogqtz.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3fkwhraxg.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3hkcnoxlc.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3jdizbrlo.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3gplyqzwv.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3bcwhjcse.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3btndgcpk.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3xwbhyrhj.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3uvameoxq.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3vkwwyhfz.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3amizjsox.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3xyshjghw.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3tkmtxudh.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3myzotkbj.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3vxemldyo.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3vkfmkqye.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3czcwscwk.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3rgbipauj.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3jdgjgrqb.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3vmogkcvx.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3pktxhfxc.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3haselwgm.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3tuyknedk.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3djhomxvr.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3coxukayf.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3bqioyxbr.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3egzashhr.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3pjmthaes.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3sajagwvk.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3ogctaupc.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3lebtprme.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3eaxzzvqw.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dkfrlzld.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3btvkzehf.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3uqbcvrmv.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3bhppanlx.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3riderlaw.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3ddchmfnm.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3wuvtiiun.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3dcjpmkav.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3sqtlvljn.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3rudhyndb.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3oofjggdm.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3dxhrcwnf.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3irnuxlns.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3aeziashg.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3wwflshxh.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3legcurkt.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3eioxvcac.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3vzybmlqw.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3nlaboche.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3iaftezcf.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3qlixfhrl.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3xlhbsduv.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3mllwjzzm.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3hlshjarw.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3irrdqmcn.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3hxlwapsc.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3mfkouffi.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3xqjefmwj.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3gjammofv.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3ibmdkdkb.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3rolxyxct.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3gghgvfsa.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3gooioxqs.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3wdjkzobo.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3gsndzkxc.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3atiitanw.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3vpmhzqfd.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3oaoiqusw.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3thnuwvzf.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3lppaymly.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3gjiykcgj.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3cenrlkmj.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3nvviryva.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3tczeztjz.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3xzlyeuhi.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3jmzgoosh.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3ltwdewts.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3gfokoudv.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3uusnqlei.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3blxtrvif.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3yrsududc.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3vxmmympf.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3fwqsoypr.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3nyqndgwj.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3bmgdfpmc.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3ooavdknw.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3iiehjmxl.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3vcdpfovr.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3dyuxnxvi.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3jnzwhzmk.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3ghcfssmw.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3nyuvjocc.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3abnakise.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3kommckba.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3akqhtuck.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3ihiknqso.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3mcfkuuqc.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3zkhyljcd.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3duozdffo.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3ebnxpakf.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3ykhtainn.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3imcvvdhy.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3kzqtviyl.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3htujofjg.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3bvzjaqzm.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3tayiqunh.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3roojwhve.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3yztqsbam.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3siphsihr.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3bglbzozi.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3bewqemhg.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3cothkihv.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3itbbmuak.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3plppgmgn.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3wwsqbhnw.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3kwhvnbxq.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3jomqykkc.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3gijrgtms.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3bmeyvduj.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3cvziknhm.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3dfqgtieh.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3ueydxyfj.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3ykrdiafk.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3qkqyxhru.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3vczcfikh.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3tspxkity.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3pzymdsfw.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3dskortrz.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3ncbfqwgw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3owlvyiwg.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3prubebvh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vqciorpr.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3wqcuqwuy.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3ephcckkp.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3bnanvqty.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3xarhfetf.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3cupfbosm.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3vgwauuew.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3ormqmhsm.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3oplzjqwz.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3rmvqrzae.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3crrtqqyx.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3lnbcvaea.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3njoarywa.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3ovkzsypb.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3hyeeimwf.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3pesyjkqg.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3xktrvnlh.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3cnsarqtl.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3egtbatmx.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3htqrxcxi.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3tzkmincz.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3tdpcrqhf.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3vgoymenx.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3rvyhmfya.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3rpdpigdh.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3jkhqeodw.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3gkexanma.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3hsxtnnyo.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3dsazioty.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3hpfdpjxc.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3slqvczly.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3locwmfzt.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3ejfehpdr.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3hhimydmq.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3xvpmurdt.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ekvryaxn.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zkimlnzk.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3lrcjetyn.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3ryzbqevi.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3hbbhesjx.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3enmhhhtu.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3fzkenjfl.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3asmzzrfz.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3jtdimthe.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3ounlagfp.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3bqlkhmls.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3ilipgyhw.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3qykrwnvv.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3pybpebrm.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3fmbvecmk.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3udcgocpf.html


<!-- 参考信息 -->