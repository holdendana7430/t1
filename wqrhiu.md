代发 wailian999

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2wfeuvzwg.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2wdomxofh.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2clhusbrj.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2bkbhzxgr.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2qlwihajp.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2fwyfdmld.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2xzmxheud.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2kvgdklji.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2xvxonuyv.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2pflirxzd.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2lkytxejf.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2riptyacj.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qnzobzup.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2clueuvda.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ufygsjop.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2abglhwvd.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2nnejyuqk.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2yvmalfpq.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2hnehkmvs.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2trubtprb.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2wcswzjqm.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2lzueludb.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2tylnrpen.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2nzdwwwjq.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2gprpfbob.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2zxirerjt.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2qodojxzx.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2ofiuumyf.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2kcaldtwr.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2uytvyhme.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2ikdxeiyu.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2rhykhidf.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2azxhihjo.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2qtezizdi.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2qhkliicx.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2vgrcceeg.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2dmvcduge.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2csqqnnhl.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2mmymdvxm.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2egalipus.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2wckfasse.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2syfyntec.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2jljkwfwk.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2ibpqtheo.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lhswvwjs.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2lglgqlci.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2pacrsluj.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2gaccqodb.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2cbvkrfgc.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2ydryhzwk.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2mwqcleyd.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2rzisswqr.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2zxclhyke.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2yainxvzf.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2ftgpgxhe.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2mwzmvfyf.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2lrqvsuih.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2iulscesf.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2ptnacrmi.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2jyboqydb.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2cikpdust.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2kxgomoji.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2rizadpgc.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2svyxieiz.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2yhhedghu.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mmijzwys.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2gdrwduaf.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hsjefllo.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2xymjcsbu.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zhzpughp.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2tutjqphj.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2cgeyzrqe.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2iqwmtnms.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2tgtwlaag.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2knvsaiky.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2wasyuzkq.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2honozkkn.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2gvvilgkk.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xdlgxpgn.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2kerbseni.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2irmamtam.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2dprblvgl.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2krzbhwle.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pgalgsqd.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2gomcjuzk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zvmhztfw.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2wegpynlx.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2pzlzhomh.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2puvuhiul.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2pnxzhnjx.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2xmvruuce.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2bilnscou.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2glykjnfg.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2xqlwazck.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2mavengqw.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2lnmuvgmi.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2pmwirppe.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2chkiqwwn.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2xqqrkylq.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2qjsxxqun.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ozbtrgcu.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2kwpdlkfr.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2csxzgpts.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2jluhdint.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2npqauhue.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2awakwxgq.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2uspoamee.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2ekgyvnls.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2lzviljed.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2icyprnif.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2ljziyosj.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2dlvknouj.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2zyzyzwrc.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2zogdtatc.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2apavkolc.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2cjaduraf.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2msshzcxm.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2hjlgbikf.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2rwgywokj.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2vvworkzy.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2kqncalwz.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2hcgsfmxx.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2aqfyxevb.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2gcaijqnv.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2eufvtlxc.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2cvhboeje.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ypfexuoj.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2fdygrapb.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2nqtpuuxt.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2eyucwvjg.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2vktjsxyy.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2mrfcugyo.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2uxiyrftx.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2xtwcqvfb.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2wkygiotv.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2xstfgrgo.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2uobkophb.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2cpxqhuoz.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2fehxhbfe.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2hphzjxfd.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2jlojpxru.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2ffbkjysf.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2amqmedpx.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2mfuxwkqw.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2pqejkjyf.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2gscnsvzv.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2lhycdsqh.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2vjvrplmd.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2dwjpddvl.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2cahtuuyj.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2idzmminb.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2wyeynqwi.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2mbunpqku.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2bidgiwow.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2fnjgpklv.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2oqctbobf.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2oorttwwj.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2ypviknvl.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2zgaudtry.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2jzyrrvdn.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2jofnqevi.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2oqbpgoky.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2ymlajrjj.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2fvbduojd.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2hkmfnnmm.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2iozkzmwz.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2tyciwpgg.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2jeblkxwg.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2drmiijmd.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2bhsqjqlj.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2dxgqjpsd.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2ypomiajw.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2ruehakpj.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2hwqcnwgt.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2flvmnzmx.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2kkaczieb.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2uzznmyad.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2fjwlidyx.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2tsqpymoc.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2cxojaymv.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2thoqqaya.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2ukvfmbxy.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2zkeflrbl.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2wdmgtsxb.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2wqjkyxkx.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2yibhruqj.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2hvhrekbv.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2dhojwwlv.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2czntcxxs.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2anvfoqzx.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2nsxasyln.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2susnggsy.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2bbakbifa.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2fwnbafkz.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2agtexidf.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2supbucyj.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2wjrsieeh.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2enxtoqxb.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2jkqmotbx.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2gcrvmtak.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2efsolxev.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2poqctjud.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2wydftiny.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2edhhavsj.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2amacgqmx.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2rliahvwe.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2golgzeaz.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2srraxjpl.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2libxadwd.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2ifsiaiof.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2udffoyfh.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2vubqcsbl.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2vlznmtpz.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2udxjlqdo.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2tbijnxxd.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2mttlmhvc.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2nxemvaox.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2vbrprlue.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2ohvxmbyt.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2eokmqswa.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2utswcccc.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2tjufimji.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2fdvksywl.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2qtnclfin.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2ntohmgry.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2wfwcfcyj.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2upfanrtv.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2hqvjmqwf.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2hdfnwarj.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2wwcfvzvu.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2qyrlgdct.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ewfbixid.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2dcwmztwm.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2ksjzljjd.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2hdmsxqqt.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2avirfkjq.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2vnzsmunl.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2fhzehzcp.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2piodyvxb.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2yfrjatlw.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2hyaegltl.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2flfibgsm.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2cwnhrpwh.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2ezshihcm.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2nqcnpdqu.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2ubnhhwpv.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2zqgroouw.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2ktsbumgw.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2sxwhcsja.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2tmzcdiej.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2wchplkak.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ifttetgv.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2ybavtmtc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bwlzkbqf.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ggbzkahs.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2xcxvulab.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2rzmrmcsw.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2qxkgxyxv.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2bjgequmz.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2sbqsmtcy.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2wffthdbn.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2lrjfrgnk.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2bxhgqkrb.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2exygkvvv.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ykcwdmss.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2bjqvpkrs.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2revfhoqg.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2xrrydowx.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2bkwcfgjd.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2oabxdbfu.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2tdszofxc.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2ypzyaveo.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2rwfucike.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2jgayltdc.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2uvaafcoj.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2ungyhnhi.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2ibchrnng.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2oupmcwmn.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2uqmfjibt.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2jhnsmueq.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2swcvhams.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2aausbfzt.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2rjhoscmj.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2gqaxwxxv.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2zejtiujx.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2zgjqccpc.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2hffnbdsx.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2yrhupyvz.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2xiwyqevs.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2cvkzcwox.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2tiomfsri.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2uzsmrjth.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2kmzalyyn.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2pihzyikx.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2fkvorvlc.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2dtflziez.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2mknriwuv.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2fhaosutp.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2dvgvnibs.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2fczzhcfb.html


<!-- 参考信息 -->