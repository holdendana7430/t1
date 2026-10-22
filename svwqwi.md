代发 wailian999

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2bciharei.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2ypyjvuff.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2wdgkwows.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2zsirebho.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2gwprgyrn.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2kqmxwchm.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2mqoephdw.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2lgcajzwy.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2eivrdame.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2tbzeperk.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2jjfkxabq.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2meslkslm.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tdhacyxx.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2umeyojmr.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2hieokxzu.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2nzgtpjei.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2fpzuagcu.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2pupptwtd.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2cbvnqtep.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2dpskimlz.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2nhixuwuc.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2bgdmroag.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2faasgbak.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2vvortger.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2svuqcgvt.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2gkidrnvw.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2nqihqypa.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2tpogewms.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2oxqppxfc.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2vvgjxaaj.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2tejzxlrj.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2tfjqpoel.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2kncobsya.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2qelmocps.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2yoldyfko.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2xwbldzas.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2vrmffqoe.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2rqvfadsa.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2tvxetxkw.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2fofyrcuc.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2bmxadfcx.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2rvrujagd.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2nwfiudoi.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2rnrqldnf.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qpunrgfd.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2atrkrefq.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2zsamtyen.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2nzapzcyc.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2cldvobiv.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2vluzdgqe.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2tvfauzdx.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2iczliylc.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2hpqbtpds.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2mtvfmkzx.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2fdxgmsii.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2xphdrapg.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2jdopmxcr.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2hebzncfd.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2tgyigvut.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2sntwkman.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2rzspuqyt.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mzzkpqzl.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2cuonmdyh.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wpbozeie.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2bhiqpqxs.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qfdwholo.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2flhtxjru.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2edxfdbtv.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2mezzivwf.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ytvuqlsw.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2tkqhipid.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2gytijurm.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2xninzfox.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2ezdrshau.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2pwixrybe.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2gbjenuzs.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2vkjxsbad.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2hrnshjkp.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hovgrfnr.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2avkployc.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2hmfxqjuh.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2evxkmsmv.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2pjlwamxb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nbvjbecf.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2yunfklbq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ctwdmwch.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2aawfcdwl.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2zpxonyvk.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2rigvovwa.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2bwxinqet.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2yznszppi.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2baninqwd.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2kvseiuxq.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2bppdwops.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2ptargrqv.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2ugtlhrop.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2ayurlqty.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2jplfzgjp.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2dsybvonc.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2gusfnhuk.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2ynjbelld.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2hbpecmpn.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2hczxqwxr.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2astyoitl.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2utcllutv.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2unqwnvzr.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2hvvfujri.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2aezxpyac.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2cydclmhy.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2hkyfhjcu.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2pgsybpdh.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2djadkwnv.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2hqtpunkz.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2yrlqzmtd.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2ecxackye.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2fpohvxnl.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2ycclgasy.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2lhkminyj.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2qxrgvwhk.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2sumuycqs.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2ddwsivuk.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2zdnbstnc.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2uvvrygld.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2azwiqtsk.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2xmkdrvih.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2ffbzwwdm.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2mwfvwcqa.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2jjfchrix.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2misbafzt.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2mrcgmupc.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2syclqyft.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2dhmmmljq.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2nodrxoiv.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2lszxoslr.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2tivqroyv.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2bhkhqvoh.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2fnsuykah.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2vslyhnjh.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2jywbftpf.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2lybxcxyx.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2frqayict.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2kcfdqqcw.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2bkcjvbkp.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2vnfxiywq.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2klidzjyx.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2phwfflkn.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2txyrplbv.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2nivkqaiz.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2fbztfriu.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2cxglpbut.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2zkhqklnr.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2jyxckppy.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2iaupiurz.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2dzazqxep.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2unhtwfll.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2dobuzsdu.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2zaggtgsu.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2cmgpyles.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2ofezilcg.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2sglnbzdg.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2nvigvabd.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2mxjymmqh.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2lnfnscdz.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2wtnolliy.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2rxngdzdv.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2uzlubnfb.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2ikwjicyt.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2dymbbhba.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2prbgloep.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2hhaswocq.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2sxsxvqut.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2bdzcuiqe.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2jphnhlih.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2dzzbcgcx.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2kbtwnyrc.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2ikyhjncl.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2supmsrkq.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2euevvlep.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2zpyjkmtm.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2ciiucppo.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2nxkvnufx.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2mdqrivoe.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2asvmsplj.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2usorfaad.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2dfwjwrpy.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2oiwsrdqg.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zdrpshra.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2tdbkabob.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2jjvvvuar.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2hblramrl.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2dmqqhsft.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2ccmspbpr.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2qzrsvmye.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2apvarskz.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2vuhhkixq.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2xksujvvr.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2cjwtecdk.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2zlqdqsgt.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ytxdmblj.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2laxgwgrl.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2rdsuxbbg.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2wcawtebu.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2lrpijkqw.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2ghwvsael.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2mlwkhpie.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2erkjfrqc.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2hnjpkaqs.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2wptfthno.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2onxeveog.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2ncsfsiac.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2pmcwmspn.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2jpzstcvq.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2nvspimtz.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2xaquoipx.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2zbiuotno.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2nyqbtewb.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2sjbkkzyt.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2dthopeul.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2gycpkwso.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2mjhulqab.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2ecnlzivg.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2qehbkcnn.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2iqdctlbd.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2jfdaauby.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2iokouvug.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2exfvwxks.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2gsbsydno.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2eznmkslb.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2ffzhlole.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2nznrkyzc.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2xzbvjabw.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2vkvvfumk.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2rszkjgwu.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2dbbhzfld.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2cdqzsfka.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2iklnmqzv.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2wtebszgd.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2svceabhs.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2kgwnwlse.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2xxvsehsg.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2zfjcguar.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2zlnzehnk.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2sqhnopzm.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2qvngduva.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2gsaqrhnt.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2yifibqds.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2warjmmel.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2rtvqcoev.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2izcrcwcg.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2uswyrdiw.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2sgzwhhxw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zdevlqpv.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2fojvtyfh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oprdnclv.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2uazhvayx.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2sztiiplm.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2mvoqfjrq.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2iwzjlvwc.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2votrpcul.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2htcmvxrm.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2gijckzbu.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2fawhrpcn.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2bqtlmmtx.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2zjlqhkiy.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2otzsyiah.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2gbxclpzc.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2cfpitksy.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2ylmebcjj.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2ojhbawaj.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2uurbxsxj.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2lejhpbwy.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2ywxzdbuq.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2qpwwjnpm.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2lfwrkxvo.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2noxuldup.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2zxzatoza.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2dlbeoxft.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2fkucmded.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2rktuqzlx.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2ksvkkyac.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2uatjyctp.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2ganuixle.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2sffdsqmz.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2afmuxmmx.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2akigrmuv.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2dqbpgcgv.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2ardqyhaf.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2oslupxtm.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2gvvltszr.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2srrwwagb.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2hbrdzqlj.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2zozgibdb.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2upzapcdm.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2uckyivfn.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2hqrdlowl.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2unejlqxl.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2ttnvnkzp.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2uotuymob.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2muwjvenv.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2ogmetbve.html


<!-- 参考信息 -->