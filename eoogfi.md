代发 wailian999

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2cqkgbycu.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2vmwewmnw.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2vrzdpahl.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2ijapmyko.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2wcioxaij.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2qfibasws.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2zyscsstu.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2elmxuhgz.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2duvdbtaf.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2iujimdrr.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2gqacirie.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2blaohjwu.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2slnyeecl.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2zqrblxqo.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2gahzopxs.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2ajiyqsqf.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2pogvqlem.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2ggbaxggd.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2yobkniuy.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2raueeezv.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2hnosbcxr.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2txfxmdev.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2gtticeit.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2onqgmfsx.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2ilgpymzs.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2wmmdtgmf.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2cpkvubfh.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2zfixndsm.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2oycmjktw.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2bjdlvhkk.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2aklixkcm.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2ykysally.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2pxswewfb.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2ogoekfur.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2yahmqfaf.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2tagktmlv.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2xhgypxup.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2zbklfsjh.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2unbgqvtp.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2wmjlfnkd.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2zzrzfkta.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2ykdjpknx.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2yivmrzcc.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2xnggmmjo.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2kktefhbp.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2bwcwbhgy.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2gvuxbmyr.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2tytswswz.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2pnncucyd.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2julybsea.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2zcfnfugg.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2cjludhxa.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2dqwjqqds.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2ljjnttzv.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2hpyoahhc.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2nocsbwdp.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2jymfshoy.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2kmlvghra.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2onnjtryt.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2kqrttikc.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2ffxzbyso.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ycvzggam.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2ffnxebyt.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ssijdyzs.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2rmonaffc.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zghlhpnd.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2mrhkqdjw.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2suegzzcv.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2kudgujgz.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fgaymqpe.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2qyzdmxzk.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2ffakebwf.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2mfjftrkt.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2dnzucffi.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2vxygxmpu.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2afzafrjm.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2jwtrecvn.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2ykjckwkf.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xrkssasu.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2kgzquvst.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2ezopgrrk.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2svjcmuyd.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2pblpcznc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qvipmnbv.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2ismfzsut.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mtemlhql.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2velzkrin.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2nbemfbhz.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2vwisgrhq.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2ohohlwqc.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2adgisnvl.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2rvkscmvz.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2vszqyudh.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2aebyrwsp.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2pmxkpobs.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2hxlobnsh.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2wdtntvny.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2swojwepb.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2aodieivs.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2crnvlbrw.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2rinjsvki.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2fyoyeynd.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2fzrucazn.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2wsdsaelz.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2okvircua.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ifnvkedy.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2prhbmuej.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2lvkcyuwh.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2dyuwykph.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2evymcane.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2svkveimn.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2oswvzpeh.html

esac
来源：http://www.52xcode.cn/Article/details/gt2pkodfhrf.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2rjfzgfmj.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2bsislgrz.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2zazurqwv.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2iutwpmwp.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2qcxtucbv.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2mqthmbsb.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2xryofeiq.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2ilxsmtmk.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2vgvkwboq.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2yksrkmis.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2slvfwapm.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2evjkxnfu.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2kzupdykg.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2ochuwcpt.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2dzfkmevt.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2xpnpmiwg.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2fupxvioz.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2ttmdcyza.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2zinposto.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2pmfhqmuz.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2snxzarux.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2riwnvwvq.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2tcyahatg.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2oxblpcdr.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2ytwxidcp.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2lcscwzmd.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2lxqinmyy.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2ifartwgi.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2npdmdyne.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2stbihnbv.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2snfeibai.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2fezhsmcu.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2tbwvqwnq.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2lknutvgn.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2pvzorpvn.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2wdnughxz.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2dcpopaeg.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2cpvqiruu.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2rwdbtaha.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2wlfycojz.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2emsdgtsl.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2lbmhjmjb.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2odxqwmkw.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2qfibnbmj.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2yoyiphov.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2gpxgmovy.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2lxxxhvbw.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2gffwfzym.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2vulpgqwl.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2woatgwpb.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2gwiltidx.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2egilarml.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2uirnazgf.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2onqgxwwx.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2pxrfdvay.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2zntcmiua.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2qhioiyov.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2gttihqpl.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2yfudhebv.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2dromtiya.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2kfrqodft.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2mqarqxbx.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2ftdxixoq.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2lusssbzb.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2luomafbx.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2syavmarj.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2wshkckry.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2utsiykri.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2tzvmetgj.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2vlfubesc.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2paejxffs.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2oaeuznkn.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2yrzpfoyp.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2frmfacrt.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2eiqpuzri.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2wqsdcrpm.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2zogphyww.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2lpcrppyl.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2psfjxwlr.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2aucfjhth.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2mrkyokyc.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2xtowdldx.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2pwxkizha.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2iyrwingu.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2bmpqoycc.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2zufqdhqm.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2phxjvjhi.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2xcqqqjdj.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2xjqilsyv.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2tundtwnn.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2tmkskqsr.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2baaxajgs.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2iwkcctig.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2hjgjxqpn.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2enkepjzj.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2qgsalbgm.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2bfihomwq.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2tvlgjyoz.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2zpzpbxni.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2xypcvisl.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2nwqdfxbq.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2bftihzxt.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2adkpcxrr.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2okbedakb.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2pxejgcfz.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2kbussprr.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2qxwhrcik.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2kjiyokni.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2ccinpxgf.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2xndqoaup.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2nvmnqnxb.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2gwqafctc.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2kalscphx.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2iupglkgf.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2zqmeqntv.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2uglljrja.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2cjyeloim.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2qggprmgp.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ntcoibvl.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2fajxytoe.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2iifhusps.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2ztqludej.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2zztofbzs.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2fwcgukie.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2mxwlxsot.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2wpsmmjyy.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2sfrjgult.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2kldqdrph.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2xqcprtio.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2nftjjznd.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2xhsuymgy.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2erdkpspm.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2nowxfvrh.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2gugcbphu.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2zxkjwawm.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2qwtktzwf.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2jhqpadch.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2muvczvzr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mnceicve.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2vxngzvzn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mlreoqlc.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2qrhxyigw.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2spsgtrmr.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2xisalvyg.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2oeptmoyn.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2wcrhvvsa.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2snngmlvh.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2ouhsnrfx.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2tgvtwwoy.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2uacpphcq.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2rioqqafd.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2mfwrpsgu.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2aexibjgu.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2pfzkrgvk.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2kcrgmlxu.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2fzojtmrw.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2zlzmwehn.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2czvgrync.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2cayqouvk.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2devhggvr.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2gsncuwga.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2clxlvdmx.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2gkuaouvx.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2bxytksbi.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2zlljmvba.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2fbddhhhs.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2wxdxnyzd.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2hkkixjeb.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2albyasbt.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2dpxoqhsq.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2kpvjjirb.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2jyloyexi.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2bqcjhgme.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2cdrrnrop.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2kjekxiyf.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2zzpluwco.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2adspzhoz.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2ewgcgswa.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2jhgbthrb.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2jpkusdtp.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2ktdpdvwd.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2yarvfkji.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2qvuyshwr.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2fwvohlfd.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2esfidlfj.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2bdiwrhgt.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2njotqaoo.html


<!-- 参考信息 -->