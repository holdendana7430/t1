代发 wailian999

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2wznokpmk.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2rgcpketv.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2fnfahwba.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2rkbntrth.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2uufwpfnj.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2cwielzds.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2incegttp.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2zlhifpva.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2sbgwlvmz.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2ktznvoaa.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2uguvfqzw.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2yzgimgit.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2xjzxbvfr.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2yyxgylnu.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2ljjyipud.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2qeftwbya.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2pxmiybbl.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2gbhhcfho.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2hifstgjx.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2imueqdkn.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2pwgeztre.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2xhxshuja.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2txzacqlc.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2gczqdtdi.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2osnexmdp.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2wmaebmvb.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2bdizkwgi.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2jllplmlt.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2kctvisze.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2ncrgnsig.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2qdwvjhoh.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2vtiozkfv.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2uvjilsea.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2gwkdlegd.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2pbhsejzl.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2klpqvtsz.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qzjojjkv.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2cegrwzrn.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2pvcyldbf.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2oygdpfph.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2qzuxhwuo.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2uyuuutze.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2hjizidzu.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2gsxlecfv.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2kmvjaprr.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2pabmvpje.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2izupvgfj.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2hlnqjikl.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2wauzbtlc.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2jpwaemsz.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2xukzqbrl.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2jcurtuus.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2tgemgrbd.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fwypscwj.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2wihhvfny.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2imzoaqwr.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2gugfbebv.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2agedgpsi.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2epyucvzg.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lnlylruz.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2kqmtewya.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lnurustb.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2uvbjjuew.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2cueuhwvp.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2hpvkpqeq.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2tztwrbfv.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2ratnjhrv.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2jecfbcbr.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2vkpcsiga.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2evravqvv.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2yfmhyuzp.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2qzmdcnbj.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2skdikmdj.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2xgfjxdum.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2vjqshgws.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ummlkpae.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2gohhuwmf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2geuzwtal.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2fitzzfrd.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2xjfsabos.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2rhicucqe.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2cljwruco.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2ckjptoke.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2qlialaph.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2reaqvtal.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2ddddxarn.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2fvlygbqb.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2kfdvwqiq.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2fnkuvbmt.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2enumyznt.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2ymienszi.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2behtggnc.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2obzktffm.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2cxdjmgkp.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ojtimupa.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2okjdalnd.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2dmkrmshz.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2rviqqvsx.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2ruyltsxj.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2vmoplwuc.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2owltnryo.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2rkezdslq.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2osejdhel.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2gzfohtnl.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2otfxzsql.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2maxkeyfu.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2qryiknuj.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2pabmtcjh.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2utmbuicl.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2pavktabi.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2rzhplhyi.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2dapcfuyr.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2ndzxwxdq.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2thxryodw.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2eikzbhgj.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2ugmrjrdm.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2cepnqdwc.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2mvrroitq.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2lykoxmhd.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2udtvdrhz.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2nstqjqsd.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2vgrvzucj.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2fwbgxsnk.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2kpkuscil.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2qobunvxj.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2vpblcdbd.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2llqadhvf.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2rwuwppbo.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2zlxawpqp.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2aiycosyc.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2konysppc.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2aypptugi.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2lpzjdvvm.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2jzkgszqf.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2libophqq.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2ydtumkrz.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2cxzozgdu.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2aqgnagyp.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2yowmiquo.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2mwbyvrkc.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2vcxpnwes.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2tjbeaoju.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2yhrgyefv.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2kiyxnfri.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kpbubiki.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2zyglrerb.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2yntejudm.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2wbvizncs.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2scmtopuc.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2hjexgotv.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2vukphtla.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2fycmzknr.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2xuhtoofs.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2ojyhlmns.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2foidcjze.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2yoinhgbb.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2pskdugtl.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2dkhwcdst.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2vkqbtxlp.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2oytskziw.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2jfzookft.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2jzdzzeqh.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2rrcnlypl.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2koqfmyyz.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2mcdrjdqh.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2vhthfbij.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2gnnxcbck.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2rubrnvsg.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2sfpxkdkr.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2kwgzggcz.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2oserodcw.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2dtcyfyoi.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2shgypdeq.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2rzzzkwls.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2wngmdfqn.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2hbckelck.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2xqmnzgdo.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2krwsvizw.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2hpcnymed.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2jeqirzoc.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2hkdfohkp.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2timpfwwm.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2rpypsjjv.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2taccjinn.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2foopnplv.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2jpxucjqt.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2kiofjqar.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2axqkwclv.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2cbymgqam.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2sgnzzdhd.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2seleoyyd.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2gtxwbyxr.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2llpmrcrj.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2bwlxrtzv.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2mrefveub.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2ndwztiuc.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2jbjcqqtz.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2asncqzzr.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2cixmacok.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2bsujbbrc.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2hmancxtz.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2mzmpxqrd.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2vfpifgai.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2tppxiybz.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2mswxuovi.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2iqrjtizx.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2cloyluqw.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2xznzfaph.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2nzplhasr.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2pgiaxbmr.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2lhkgaarm.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2kicwghrq.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2dmyrzvca.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2nxcyrluy.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2igflqctk.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2cwthfmox.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2ajsxwigq.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2rprgqwzo.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2ihdaqgrl.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2rikyvhwf.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2qthdtusd.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2oexbgugd.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2ldjtbcpf.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2ntpxgkwm.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2dtwegkuq.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2mybsscnr.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2pxazeikx.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2iuujhfcw.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2eoorpyry.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2rwnxwjmj.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2qhqqityz.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2znrkyetr.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2bstvypur.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2hctbqpkv.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2sccgdmez.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2sbtezabk.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2dxnkhgwr.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2opweetwt.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2htrzgfmv.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2qwipwxvg.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2cdurxzlc.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2zskjbfck.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2acebrzjk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2feaywrsr.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2ugvrnkrw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wgjjgrlp.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2tmjhujav.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2bqvmvixs.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2adbjlbru.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2ejxpcezw.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2zfpnvpbn.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2vhvjktkt.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2cdfozmrr.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2lktenxjt.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2tpnjfkdi.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2ttzjbkxu.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bwzldish.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2fixlyeqh.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2diuxvsxc.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2uxtffjpz.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2gvwwekfr.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2aztsjnnd.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2qgpchjvf.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2ptuxliqi.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2tknbfxoc.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2hzfqxxsy.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2jmdlcyfy.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2oiikbnnk.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2cdctjqoe.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2kppdastc.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2nwjkpjix.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2suzaobwu.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2sexyykxj.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2pkyhpddb.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2ngafvtvz.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2eolvekwc.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2dlhidrrx.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2tncecqes.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2ctzwrpxe.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2bvhdgitr.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2alhcmocx.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2iogtidtn.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2jlrmwihg.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2lholoxbb.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2qtzfrhre.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2opclbmji.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2qmdztzku.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2mborzwea.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2sfaulqfp.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2qpbvdfke.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2eevrbrxf.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2kfoxywqs.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2ykwekpmf.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2odmyigzl.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2ngwbgqmk.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2mhrxxghb.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2hthqqvpv.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2daofmnow.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2bnrswbci.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2nlrobppg.html


<!-- 参考信息 -->