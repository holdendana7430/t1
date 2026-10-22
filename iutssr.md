代发 wailian999

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2cbljxiwx.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2xfyrpckp.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2dbhrpisy.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2dqljdoia.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2iclefnnm.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2wemhoskn.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2rvmdojah.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2nvitabew.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2crmjqliv.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2aqijhpnt.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2fuhlnirt.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2nflxocsf.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2szuzbyvk.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2mjlhxfnm.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2bjwszgcd.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2yachsorl.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2umhcfekm.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2xkfcrnhl.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2peosmnax.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2yueqeujz.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2quhsfvgy.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2muxghxpq.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2xpygsqzu.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2azsmofxx.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2kjtignyb.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ggcdzequ.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2fnsgoffu.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2azqubpcj.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2yjqwyepg.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2acasjlmt.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2jqqpxqht.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2ewxxedir.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2wqxjstnb.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2axxcngef.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2jcumimkx.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2lbnftgst.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2vqnbduho.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2bmuyamgr.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2qjeuccsl.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2fcrcejzl.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2gnfyzylc.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2vwpthhgn.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2opgctyza.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2shwvrivi.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2lozkjkny.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2fsmkcgix.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2ftpdrhbe.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2fnipilhe.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2odkaqryg.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2gheajxqb.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2cgquitvo.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2uccxyezv.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2btbkrghm.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2rnmqiepl.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2udwqufrw.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2cvauxlrx.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2tejcsibm.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2byldoujq.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2oavpzmuv.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2dshydoqu.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2erwensqg.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2dcmlnycd.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2elfimhkl.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2nheyvvxk.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2alnpuscz.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2puigbqvl.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2upxzsnwa.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2uedttcfs.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2bgsygchs.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2naqjagvc.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2toxoyqws.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2pepnhqsa.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2szypfvyr.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fqdltxjc.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2ogyauvlk.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2qziqayqi.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2mbvaiutz.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2ktvkyskc.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2xbggfrwh.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2jorlijbk.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2ygoqsmpr.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2hubitkpc.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rlhuowai.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2cqnxtylq.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2teeqavvs.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2hvnqvhxb.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2tjthdqjb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ddgmbxjr.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2pjmslvwe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ubduvsnu.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2xponvdof.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2howpelwm.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2xuvftogt.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2fijpuhhf.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2qtauquek.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2jyyidqcz.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2wibhdjyi.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2pkxsunbt.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2ikefbdwq.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2sbkelnbf.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2kzfkocdy.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2iidarfjl.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2wjxbkcrc.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2yndxtllk.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2tghahtjs.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2ypfcblyp.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2evultypt.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2qkhcxgin.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2lvrhrlxj.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ioclewyb.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2aturmsen.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2onjqxfgg.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2bzfrfoyy.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2lstjwsqf.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2njihkwoe.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2gsxqifat.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2hdysjpno.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2kvnqxfle.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2wsjroyto.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2jsupfdpc.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2aubwgoav.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2efrcuton.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2tsrmhpou.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2lncnnuew.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2qrzyyzbs.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2ifgzrmzd.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2myqpeteo.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2xgrcdlrf.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2nxcsqglw.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2xhcvwpcd.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2yixkucdh.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2ukyvyyur.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2usngwlzp.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2idknymdr.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2rayfrqqu.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2dhafwknw.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2nkvimigl.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2qcnkvjia.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2xubuqahb.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2aeioczar.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2dxsadhzx.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2kixslhkg.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2dawacrdj.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2dpayxrky.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2xwohbley.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2wrzpijwn.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2qgrtwnom.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2lrbgohcu.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2tddvyjzu.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2chvyzjdy.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2iqxryyjn.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2ssdoiovz.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2wrnrhkye.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2sppmjecu.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2dyjsctbd.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2ajmhtlul.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2vvltzpbz.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2suixkhvl.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2hczjwehg.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2pzxcuemx.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2qnqgrrqr.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2wiqlvgyq.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2mmzkmstu.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2wghzwogm.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2ajaormze.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2zbnxbrgh.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2xjvrsicq.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2hnhrheic.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2mgnyalel.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2lwvrylqp.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2orlexqun.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2lqbhfvqg.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2yqghpnla.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2uopaguaw.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2jugqrery.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2hrkaoxxd.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2jbvbliup.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2jnmtehsw.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2axxgebep.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2jiswhlrp.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2wkchdfwv.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2zlqmjzvr.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2yjrtrxxr.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2dmnlhhpa.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2nqamxkzr.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2sobcvyno.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2qnpmzpbm.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2mmtioyxe.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2pzwxpmdi.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2oovgtcme.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2oqphmeeu.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2cxdwupkv.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2vtrcuyvm.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2zuuymkau.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2soxzmtty.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2njhfbdbg.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2knzekylg.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2syqaemov.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2lezjnbwb.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2uutxalti.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2rajunwbn.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2aaxuonch.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ppouweye.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2jjsdgqca.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2jxlmntyj.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2nmayekvw.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2osxtfqba.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2lwfyebdn.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2fbhjlxnn.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2sxlxnmkp.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2yybsxjxz.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2fikmdjbu.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2rrpnhbqi.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2prabxoid.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2zxhdbtia.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2fanbcuvu.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2xwjxkkdw.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2xuossmia.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2nvxmhbuq.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2fqmlxjca.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2ldzjyylt.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2inapzhry.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2qwekrxbm.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2drrkpekv.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2uvqgwiys.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2xbsloaxa.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2dqvwlmlx.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2ucpswskl.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2ryqearqa.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2udhfhihm.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ayzffgos.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2kulvdaah.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2ovyofcyo.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2aorcvtvm.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2iqaycxvk.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2xldjdqqn.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2zalcmkma.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2dzntorlj.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2zkvmphmv.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2foriuzkv.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2mmfpupbn.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2ytbrtwph.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ixzcxkeh.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2zlbgkfqc.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2lfcebcjg.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2qxcmvfjw.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2tjlxonnb.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2lrzfuzrs.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2bcgixgyz.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2qmphkzdl.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2pgtuxsse.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2ccbwaljp.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2vmvenmme.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2waeujksw.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2orsqnbhm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ioafaocs.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2xgzsdyiz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oognwkov.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2tjwzepgk.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2awmfezlj.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2teearbux.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2ozgcidad.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2rpmxzzbv.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2rutyeacl.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2hglkjcgp.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2djxdqwvs.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2tyqjjxfa.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2neapnrno.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pnnfegek.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2pjwdjnpy.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2oiiurypr.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2vebcshde.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2zpeycgnb.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2cdplibae.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2izuobdwz.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2ndaliteu.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2fbfcitos.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2frxarayb.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2lafzuovr.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2sxwdhwvc.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2xmhyrwnd.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2ykbepesj.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2goncetoj.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2kjtoyutn.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2dtuskpab.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2tpcspjvd.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2otilqagc.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2vuhfjgfo.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2kfomfdap.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2pfbdezbf.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2izqeihlv.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2tvgkqnsx.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2fgwcaxaq.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2fcfhdzwl.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2twkwnypu.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2mninxxfj.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2dtskboiy.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2brfordti.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2hbcnfldb.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2rohyfize.html


<!-- 参考信息 -->