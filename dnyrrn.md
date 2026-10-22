代发 wailian999

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2wgaqrnfw.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2obbaznfx.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2qizyyrcz.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2imiyegkd.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qjsnvwui.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2bmsasnom.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2jzqrgpfc.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2abaywsjg.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2dmtnfiab.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2fjkhcezl.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2aqlijmdj.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2bxzynpxe.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2mlnlyoez.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2fatfbmkg.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2jtizvgrq.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2lrabinqu.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2vqvledbx.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2kkqdpbnf.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2gjnzkqsb.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2bomafzlf.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2ulsqmwzc.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2vjyympjs.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2tbfjndlt.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2bphymvkb.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2tekoegfg.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2owtnbdcd.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2shihxojf.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2qzhvhmoa.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2hqpihsiq.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2vegjgacb.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2fpcujimb.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2espgcnun.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2lmspuqgg.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2qqgfeuuj.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2rxvhzvfr.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2erogfocw.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ykuaoufy.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2xypiocto.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2ibpfeske.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2zwjlgqjo.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2puigbqvj.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2hexmmooo.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2mnyfnvlx.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2etwcmhdb.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2otnbujln.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2ftkgcagi.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2wqsxjlwq.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2jxrfzhwj.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2pxlvwfdh.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2wimpppjm.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2qroicayx.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2ktjnlinb.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2ikmrxpfq.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rnklxsrq.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2upxibsfy.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2uzvcuxkv.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2dezlhudk.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hrrtldll.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2hekyqkoz.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vjxndydd.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2gefjbkwb.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fotgdrpt.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2efdxufsj.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2axgxuruj.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2gktkadfz.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2dtqntdbs.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2lisinyau.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2inghotic.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2abfpwchm.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2wmjvmsoo.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2halpxrsq.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2hippvzrz.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2vlveyldk.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2nhitvzhb.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2qlcbtqyy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2swpilstm.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2xciozpjq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cqfpumog.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2cusomfwl.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2omsujmpx.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2reiqwekd.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2kztbueij.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2qffosrqo.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2fsvfbyhm.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2tbamlpis.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2yjcmvord.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2dwwaonnf.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2lqpuzbvu.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2viqnlhjb.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2xeaorhze.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2kewstvkf.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2nioxrbqk.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2lstbbrcm.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2loyljzpp.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2yhndymxb.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2auiuddmp.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2sukdtqzk.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2xpdmsmuf.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2busqebsg.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2vhhrqnby.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2znfhorxg.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2ivgphsyk.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2jxwiyndw.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2vbgmnxto.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2bzxffjty.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2puqddnav.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2ozhdjxst.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2imajdshc.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2mvscocon.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2jmxzyaek.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2znlrlsje.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2nbkforgc.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2yceezluq.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2rqchznlb.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2dtiplsrv.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2mwkdtgvb.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2xhelzqfz.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2dkqmedia.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2qqrvgwee.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2fpxixorb.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2vgbazbiz.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2logwrkue.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2krvroeuz.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2nydxqioa.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2bzplizsc.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2ighuoadd.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2jcctilfp.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2axnafhvz.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2mmaluilw.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2nmarwgfd.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2fdhimzpj.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2ehhjthxm.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2xrjhfyds.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2wsrnlbfc.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2xennehxf.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2dinhhhyo.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2woqjwrbz.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2bhchlxvi.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2clxhlhmv.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2kdobdfhh.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2evuqrgav.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2kjafbuxw.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2gvuksmhh.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2gaffyujn.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2iwhxhjcz.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2zdrriopd.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2ekxveblm.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2yypbumdi.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2mjhyssdo.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2vgotyxqi.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2eysctbbh.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2owyaijkp.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2izyoryjs.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2kpvvorad.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2kxovywfe.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2pcrzjktj.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2aesrjtiq.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2mgdpmtgj.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2odentswv.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2xkzlcibm.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2dukfdgxq.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2zvzbrqfx.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2ovmurlhj.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2hubhcnhs.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2uvyhqlfx.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2feqfjqwk.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2iasbbigs.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2vthqdvlh.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2dvuuogpi.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2jhszphdu.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2fjnapkvy.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2cwshpssh.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2kwgrmcla.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2ziosjzpg.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2ucvqqibk.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2lkexumlm.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2xhovzyis.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2rlfrcvvk.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2svmlqfzq.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2cillstsf.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2aaugfdmt.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2zfzcileu.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2kpxbtoco.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2gkvjmhkm.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2jikgkqlh.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2atwjjgmr.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2eyeoskpg.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2lopvwdkv.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2xovbezgx.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2ykmieqmg.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2vqkpjeyf.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2gzeekmcn.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2ugyljctj.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2bycwythe.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2isowcdpi.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2rnaygleq.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2iezyjfed.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2pxzjrrlo.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2btqdwtyj.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2bgwhoqbd.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2zdymvcfe.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2zjsiqgod.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2helqexlc.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2yzyvuslg.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2bheyzjhr.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2drbcbxie.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2ubffjwzv.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2bncgleag.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2hzyveicz.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2nokcrqaz.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2cjbskamk.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2dbziuarx.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2bgamonfw.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2fsplzird.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2umnnbbaq.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2blkgwclz.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2epdyprai.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2iwiqtpoa.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2jdxckckx.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2pxvfglww.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2zxmobprr.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2qgxjrxiv.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2qcosocwq.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2jkotvonx.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2ptrybrah.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2kjairzyc.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2ltcnqoqi.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2hwljnzhh.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2pxouwfrr.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2egrowcla.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2abuvrrey.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2oouhvsjh.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2nvvzsiio.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2dclakkyf.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2cnydmjol.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2fxsyokof.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2dsitknbe.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2cmbcfzey.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2zeozxwnn.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2htuymten.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2idwcskbl.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2szxyjnzp.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2kyqxwojp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pvhjgmvt.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2ypkoduos.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kdahsvws.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2sxesmfjj.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2ldxtocvk.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2ifzyscud.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2tjbcliay.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2fnaimopj.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2svzfltbe.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2hwfzoxpb.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2kcgmykuu.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2ukfnibkb.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2qenlmuxa.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2uuzciokn.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2zfnunwbz.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2wcxetnkr.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2qboxkjjc.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2nrlomfoy.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2netegyty.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2ofldrazn.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2hlqxwhtt.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2dokrrltb.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2evouchjf.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2duhnjpuz.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2qqfbfrpl.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2lsrffpip.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2nbnccktj.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2bvjckkbk.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2yrpmxbgw.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2aqkrjyyd.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2bprxxtau.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2ybbscjlg.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2xcroijsg.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2xktnatiy.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2zcugqrrz.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2dzyuambx.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2ddtliaze.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2lkmdmwcn.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2exdototq.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2lfhnzkzf.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2gagckdnr.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2ifwtlvbq.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2xiztucsl.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2qrplulpz.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2ulnhspqr.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2glrnszfc.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2rfeleujv.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2ljjdking.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2qjyazyjd.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2nkkxphdg.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2zeoqfpvh.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2qxtwkray.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2gmzspasm.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2aesniwvv.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2qkyblfzr.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2udbafxiw.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2xuaqgdyp.html


<!-- 参考信息 -->