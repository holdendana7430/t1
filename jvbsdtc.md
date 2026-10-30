代发 wailian999

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.zdbjq.cn/Article/details/govxlytzl.sHtML

[Q50] 批量更新
来源：http://wap.hesvh.cn/Article/details/gfzapzcoh.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.zdbjq.cn/Article/details/gegqmhabx.sHtML

[Q51] 用子查询更新
来源：http://www.share.fehbvm.com/Article/details/gfouscqez.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.hesvh.cn/Article/details/gxkuahyli.sHtML

[Q52] 删除指定行
来源：http://baike.fehbvm.com/Article/details/gvttabcwj.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.hesvh.cn/Article/details/gmjdeefvi.sHtML

[Q53] 按条件删除
来源：http://mobile.hesvh.cn/Article/details/glxdlcjxl.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.hesvh.cn/Article/details/gzqlcfkts.sHtML

[Q54] 清空表
来源：http://www.m.share.fehbvm.com/Article/details/gcxsfoddi.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.hesvh.cn/Article/details/gjcgugvrp.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.hesvh.cn/Article/details/gzncvhmqd.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.fehbvm.com/Article/details/gbqzyarsb.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.zdbjq.cn/Article/details/ggorpfhju.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.fehbvm.com/Article/details/gegzljjcx.sHtML

[Q57] 行号
来源：http://mobile.fehbvm.com/Article/details/grcuelpaz.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.zdbjq.cn/Article/details/gvibvpnvx.sHtML

[Q58] 累计求和
来源：http://baike.zdbjq.cn/Article/details/gevaiywmp.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.fehbvm.com/Article/details/grqvckcqf.sHtML

[Q59] 分组内累计
来源：http://read.share.zdbjq.cn/Article/details/grvzngihg.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gdlhndsvj.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.zdbjq.cn/Article/details/gtvgtprot.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.fehbvm.com/Article/details/grblrhqie.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gxotjsial.sHtML

[Q61] 移动平均
来源：http://www.share.fehbvm.com/Article/details/gwxykcgzt.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gesmfarih.sHtML

[Q62] 分组占比
来源：http://read.share.zdbjq.cn/Article/details/gvqhxcpgu.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.hesvh.cn/Article/details/gwoqgqgkg.sHtML

[Q63] 开启事务
来源：http://www.m.share.zdbjq.cn/Article/details/grhrsawkf.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.fehbvm.com/Article/details/gzxjzvwqv.sHtML

[Q64] 提交事务
来源：http://3g.zdbjq.cn/Article/details/gxeqzztnl.sHtML

COMMIT;
来源：http://mobile.fehbvm.com/Article/details/gdlhlmapk.sHtML

[Q65] 回滚事务
来源：http://www.share.fehbvm.com/Article/details/ggyfowuyc.sHtML

ROLLBACK;
来源：http://blog.fehbvm.com/Article/details/gbibrwrky.sHtML

[Q66] 行锁查询
来源：http://www.share.zdbjq.cn/Article/details/giyyycsqp.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.fehbvm.com/Article/details/gsgcrtywx.sHtML

[Q67] 设置隔离级别
来源：http://baike.fehbvm.com/Article/details/gfbajgewf.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.hesvh.cn/Article/details/gfhkykkiv.sHtML

[Q68] 保存点
来源：http://www.m.share.fehbvm.com/Article/details/gevleztgh.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.zdbjq.cn/Article/details/gohnblfds.sHtML

ROLLBACK TO sp1;
来源：http://read.share.zdbjq.cn/Article/details/ghofbndap.sHtML

[Q69] 查看执行计划
来源：http://mobile.hesvh.cn/Article/details/gshqtqyty.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.hesvh.cn/Article/details/grdthhskk.sHtML

[Q70] 更新统计信息
来源：http://3g.fehbvm.com/Article/details/gubyvwgaw.sHtML

ANALYZE TABLE users;
来源：http://mobile.fehbvm.com/Article/details/giallgyep.sHtML

[Q71] 查看建表语句
来源：http://read.share.zdbjq.cn/Article/details/glucbrrkr.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.hesvh.cn/Article/details/gzsptpltm.sHtML

[Q72] 查看索引
来源：http://www.share.hesvh.cn/Article/details/gamkrruxg.sHtML

SHOW INDEX FROM users;
来源：http://m.share.hesvh.cn/Article/details/grhyxcouf.sHtML

[Q73] 查看表状态
来源：http://3g.fehbvm.com/Article/details/gtnbilflk.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.hesvh.cn/Article/details/gpyfdpgkr.sHtML

[Q74] 强制使用索引
来源：http://m.share.zdbjq.cn/Article/details/gguoflzfh.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.zdbjq.cn/Article/details/gbktvafgg.sHtML

[Q75] 日期格式化
来源：http://read.share.zdbjq.cn/Article/details/gvxkpvzya.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gdllquocw.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.zdbjq.cn/Article/details/gdetymgqv.sHtML

[Q76] 按天统计
来源：http://m.share.fehbvm.com/Article/details/gnyzfitae.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.zdbjq.cn/Article/details/gxyamrvxs.sHtML

[Q77] 时间加减
来源：http://www.share.hesvh.cn/Article/details/ggytwkzip.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.hesvh.cn/Article/details/gizfikrny.sHtML

[Q78] 当前时间
来源：http://www.share.fehbvm.com/Article/details/gvooyshji.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.zdbjq.cn/Article/details/gmxmkpvbc.sHtML

[Q79] 字符串拼接
来源：http://www.blog.hesvh.cn/Article/details/gjskdgbxl.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.zdbjq.cn/Article/details/gcvmejrjc.sHtML

[Q80] 字符串截取
来源：http://www.share.hesvh.cn/Article/details/giyqhnlbj.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gwzhtgens.sHtML

[Q81] 字符串替换
来源：http://www.blog.zdbjq.cn/Article/details/gnpdtcxwx.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.hesvh.cn/Article/details/gpyahlyah.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.fehbvm.com/Article/details/gzymomgos.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/griiziang.sHtML

[Q83] 大小写转换
来源：http://wap.zdbjq.cn/Article/details/guxignnny.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gcodjtdjf.sHtML

[Q84] 去除首尾空格
来源：http://read.share.fehbvm.com/Article/details/grqqgewjb.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/gznxaqkna.sHtML

[Q85] 数值取整
来源：http://www.share.hesvh.cn/Article/details/ggmwyhzzd.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.hesvh.cn/Article/details/gsqqzuswo.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.fehbvm.com/Article/details/ghcbojiti.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.zdbjq.cn/Article/details/gyxsilidk.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.fehbvm.com/Article/details/gvjlvmuyl.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.zdbjq.cn/Article/details/gwfyrpofw.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.hesvh.cn/Article/details/gyvgqudvb.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.fehbvm.com/Article/details/gnyopsqzq.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.fehbvm.com/Article/details/gwnkkwlav.sHtML

[Q89] 判断表是否存在
来源：http://www.share.zdbjq.cn/Article/details/gjymqrdma.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.fehbvm.com/Article/details/gplshiqag.sHtML

[Q90] 生成序号列
来源：http://3g.fehbvm.com/Article/details/gmphhmifq.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.hesvh.cn/Article/details/gkmxamglp.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gyiadtstt.sHtML

R. Bash 专题
来源：http://baike.hesvh.cn/Article/details/gwabkytot.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gssloqxqf.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.fehbvm.com/Article/details/gvgarbmzf.sHtML

#!/usr/bin/env bash
来源：http://3g.zdbjq.cn/Article/details/gspijotob.sHtML

set -euo pipefail
来源：http://read.share.fehbvm.com/Article/details/gnjgbcwae.sHtML

[R02] 变量赋值与使用
来源：http://blog.hesvh.cn/Article/details/gznlzqqcs.sHtML

name="Tom"; echo "$name"
来源：http://baike.hesvh.cn/Article/details/gcekslzve.sHtML

[R03] 只读变量
来源：http://mobile.fehbvm.com/Article/details/gtxegykdo.sHtML

readonly PI=3.14
来源：http://3g.fehbvm.com/Article/details/gezaicsud.sHtML

[R04] 位置参数
来源：http://www.share.zdbjq.cn/Article/details/giiqbiehc.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.hesvh.cn/Article/details/gjbsjhlve.sHtML

[R05] 参数默认值
来源：http://mobile.zdbjq.cn/Article/details/gcouqphrx.sHtML

name="${1:-default}"
来源：http://3g.fehbvm.com/Article/details/gitmmkfkt.sHtML

[R06] 判断命令是否存在
来源：http://read.share.hesvh.cn/Article/details/gxpskxvvo.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.hesvh.cn/Article/details/gysenleur.sHtML

[R07] if 判断文件
来源：http://baike.zdbjq.cn/Article/details/gzqapataf.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.zdbjq.cn/Article/details/gynjuglwi.sHtML

[R08] 数值比较
来源：http://wap.zdbjq.cn/Article/details/gcivlbnqh.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.zdbjq.cn/Article/details/gkskrwkyo.sHtML

[R09] 字符串比较
来源：http://wap.fehbvm.com/Article/details/gblgkbayw.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.hesvh.cn/Article/details/ggzpjzeoq.sHtML

[R10] 正则匹配
来源：http://www.blog.zdbjq.cn/Article/details/gspahjzvd.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.hesvh.cn/Article/details/gapavnhux.sHtML

[R11] case 多分支
来源：http://3g.fehbvm.com/Article/details/gewrmhxys.sHtML

case "$1" in
来源：http://www.share.hesvh.cn/Article/details/geylcbqkf.sHtML

start) echo "启动" ;;
来源：http://read.share.fehbvm.com/Article/details/gzujetjfz.sHtML

stop)  echo "停止" ;;
来源：http://mobile.fehbvm.com/Article/details/gojfoponf.sHtML

*)     echo "未知命令" ;;
来源：http://wap.fehbvm.com/Article/details/gidgblldz.sHtML

esac
来源：http://www.blog.hesvh.cn/Article/details/ghddhgepe.sHtML

[R12] for 遍历文件
来源：http://www.share.hesvh.cn/Article/details/gzoumvrln.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.zdbjq.cn/Article/details/gtvskqcvw.sHtML

[R13] for 计数循环
来源：http://mobile.fehbvm.com/Article/details/ggtiwwhsv.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.zdbjq.cn/Article/details/gsyrnxonf.sHtML

[R14] C 风格 for
来源：http://www.share.zdbjq.cn/Article/details/gpuzdwqsz.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.fehbvm.com/Article/details/geotbizdd.sHtML

[R15] while 逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gcnqjusji.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.fehbvm.com/Article/details/gpycytkvw.sHtML

[R16] until 等待条件
来源：http://www.blog.hesvh.cn/Article/details/gqgfvyyzy.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.fehbvm.com/Article/details/ghvafaayz.sHtML

[R17] 数组定义与取值
来源：http://www.share.hesvh.cn/Article/details/gljczjxxx.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.zdbjq.cn/Article/details/gnuzdhqxg.sHtML

[R18] 遍历数组
来源：http://wap.zdbjq.cn/Article/details/gktxqfzzl.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.hesvh.cn/Article/details/giwshflvd.sHtML

[R19] 数组长度
来源：http://www.share.zdbjq.cn/Article/details/gnucfcbbi.sHtML

echo "${#arr[@]}"
来源：http://mobile.zdbjq.cn/Article/details/gftuoeflx.sHtML

[R20] 关联数组（字典）
来源：http://mobile.zdbjq.cn/Article/details/gymchxudx.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.hesvh.cn/Article/details/gtgdiibpp.sHtML

[R21] 字符串长度
来源：http://www.share.zdbjq.cn/Article/details/gbwleohia.sHtML

echo "${#s}"
来源：http://read.share.hesvh.cn/Article/details/ggypjhqgc.sHtML

[R22] 截取子串
来源：http://blog.fehbvm.com/Article/details/gopguztuu.sHtML

echo "${s:0:5}"
来源：http://baike.zdbjq.cn/Article/details/gctwaqfcv.sHtML

[R23] 字符串替换
来源：http://baike.hesvh.cn/Article/details/gzwjxduue.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fehbvm.com/Article/details/gjzlvjfpp.sHtML

[R24] 大小写转换
来源：http://blog.hesvh.cn/Article/details/gguwmzfhz.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.fehbvm.com/Article/details/gvzsncdce.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.fehbvm.com/Article/details/gdtebxpum.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.zdbjq.cn/Article/details/genmlfzof.sHtML

[R26] 命令替换
来源：http://blog.zdbjq.cn/Article/details/gqhreheww.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.fehbvm.com/Article/details/gbvskbmhk.sHtML

[R27] 算术展开
来源：http://www.blog.hesvh.cn/Article/details/govevcyap.sHtML

echo $((1 + 2 * 3))
来源：http://baike.zdbjq.cn/Article/details/gqcezjmio.sHtML

[R28] 浮点运算
来源：http://www.blog.hesvh.cn/Article/details/gtpzbjwyo.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fehbvm.com/Article/details/gcgoxxiyb.sHtML

[R29] 定义函数
来源：http://wap.hesvh.cn/Article/details/gwbseaqjj.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.hesvh.cn/Article/details/ghbhxmshw.sHtML

[R30] 函数返回状态码
来源：http://wap.zdbjq.cn/Article/details/gbwkjhlet.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.zdbjq.cn/Article/details/gjiegjxxb.sHtML

[R31] 局部变量
来源：http://wap.hesvh.cn/Article/details/ggtftvyov.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.hesvh.cn/Article/details/gcvvycuhk.sHtML

[R32] 参数个数校验
来源：http://www.m.share.hesvh.cn/Article/details/gyqjsepnz.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.hesvh.cn/Article/details/gmxcecidu.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.zdbjq.cn/Article/details/gmqwhyqqw.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.fehbvm.com/Article/details/gtsepkquq.sHtML

[R34] 退出时清理
来源：http://read.share.fehbvm.com/Article/details/gagvnfngh.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fehbvm.com/Article/details/gsjimoiwg.sHtML

[R35] 后台执行并等待
来源：http://baike.fehbvm.com/Article/details/grqyngoxr.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.zdbjq.cn/Article/details/guqzyolgq.sHtML

[R36] 并发执行多个任务
来源：http://3g.fehbvm.com/Article/details/gyfneivrv.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.hesvh.cn/Article/details/gpblexovp.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.zdbjq.cn/Article/details/gizehbsnr.sHtML

files=$(ls -1)
来源：http://www.m.share.fehbvm.com/Article/details/guzngfuhd.sHtML

[R38] 管道串联
来源：http://read.share.fehbvm.com/Article/details/glnoigrba.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.zdbjq.cn/Article/details/gmugfodxa.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.fehbvm.com/Article/details/ggqkcdzoz.sHtML

cmd > out.log 2>&1
来源：http://m.share.hesvh.cn/Article/details/gbboparlu.sHtML

[R40] 追加写日志
来源：http://www.blog.hesvh.cn/Article/details/gxnzsaqfi.sHtML

echo "log" >> out.log
来源：http://3g.fehbvm.com/Article/details/gfdbfjoik.sHtML

[R41] 丢弃输出
来源：http://blog.hesvh.cn/Article/details/gintqyjsz.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.fehbvm.com/Article/details/gqtzknnzt.sHtML

[R42] 输入重定向
来源：http://blog.hesvh.cn/Article/details/gquktpptr.sHtML

wc -l < a.txt
来源：http://m.share.zdbjq.cn/Article/details/gbcxiruoc.sHtML

[R43] 按名字查找文件
来源：http://mobile.hesvh.cn/Article/details/gjoycescg.sHtML

find . -name "*.log" -type f
来源：http://www.blog.fehbvm.com/Article/details/gpnfwfkji.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fehbvm.com/Article/details/ggcnqodrm.sHtML

find . -mtime -7 -type f
来源：http://www.share.fehbvm.com/Article/details/gtthwjdbi.sHtML

[R45] 批量删除
来源：http://www.share.zdbjq.cn/Article/details/glrmawzri.sHtML

find . -name "*.tmp" -delete
来源：http://blog.fehbvm.com/Article/details/gtdacswav.sHtML

[R46] 递归替换文件内容
来源：http://read.share.hesvh.cn/Article/details/gythkzcxw.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.hesvh.cn/Article/details/gkkjsvjnm.sHtML

[R47] sed 单行替换
来源：http://read.share.zdbjq.cn/Article/details/gwgpcvbdr.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.zdbjq.cn/Article/details/guezhaopb.sHtML

[R48] awk 取指定列
来源：http://wap.fehbvm.com/Article/details/gjdjmjdrt.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.zdbjq.cn/Article/details/gwkqzmttg.sHtML

[R49] awk 带条件
来源：http://read.share.zdbjq.cn/Article/details/ggrnamxcy.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.fehbvm.com/Article/details/gdyjxvpjk.sHtML

[R50] awk 求和
来源：http://www.m.share.hesvh.cn/Article/details/gmkkpprrn.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.fehbvm.com/Article/details/gafgiqcgc.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fehbvm.com/Article/details/gwutykrzf.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.hesvh.cn/Article/details/gjpmrqjal.sHtML

[R52] 统计行数
来源：http://www.blog.hesvh.cn/Article/details/gehxjnluw.sHtML

wc -l a.txt
来源：http://www.share.fehbvm.com/Article/details/gsgjrhcgq.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.zdbjq.cn/Article/details/guidjvghu.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.zdbjq.cn/Article/details/gppuntsgd.sHtML

[R54] 比较两个文件
来源：http://www.share.fehbvm.com/Article/details/gvldgxsew.sHtML

diff a.txt b.txt
来源：http://www.m.share.fehbvm.com/Article/details/gjhqryyic.sHtML

[R55] 压缩与解压
来源：http://3g.fehbvm.com/Article/details/gaspzrecn.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.hesvh.cn/Article/details/ghypwnavu.sHtML

[R56] 远程拷贝
来源：http://www.m.share.hesvh.cn/Article/details/gmbhilisz.sHtML

scp file user@host:/path/
来源：http://m.share.fehbvm.com/Article/details/gcdfjluny.sHtML

[R57] 远程执行命令
来源：http://www.blog.zdbjq.cn/Article/details/gezzuqtyq.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.zdbjq.cn/Article/details/gxhjvmeto.sHtML

[R58] 下载文件
来源：http://www.m.share.fehbvm.com/Article/details/gbrmhcuzr.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.fehbvm.com/Article/details/gsftnzuoe.sHtML

[R59] 发 POST JSON
来源：http://wap.fehbvm.com/Article/details/gahfmrwjh.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.fehbvm.com/Article/details/gisleqsck.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fehbvm.com/Article/details/gwxadtgyd.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.zdbjq.cn/Article/details/gaejnnbgj.sHtML

[R61] 磁盘占用
来源：http://3g.hesvh.cn/Article/details/govkuhoxy.sHtML

df -h;  du -sh *
来源：http://blog.zdbjq.cn/Article/details/gnuqtbjyr.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fehbvm.com/Article/details/grphqwiyc.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.zdbjq.cn/Article/details/gwfcjenry.sHtML

[R63] 内存与进程
来源：http://www.share.zdbjq.cn/Article/details/gugwsicxu.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.hesvh.cn/Article/details/gfvbfhwix.sHtML

[R64] 结束进程
来源：http://www.m.share.hesvh.cn/Article/details/gptlnxqwa.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.fehbvm.com/Article/details/gdwojtrsm.sHtML

[R65] 查看端口占用
来源：http://baike.hesvh.cn/Article/details/goshwcuuf.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.zdbjq.cn/Article/details/ggzkqczcc.sHtML

[R66] 定时任务
来源：http://www.share.zdbjq.cn/Article/details/gnxbuoktq.sHtML

crontab -e;  crontab -l
来源：http://3g.zdbjq.cn/Article/details/gzzzxtbnl.sHtML

[R67] 生成随机十六进制串
来源：http://3g.zdbjq.cn/Article/details/gjksmcvdw.sHtML

openssl rand -hex 16
来源：http://mobile.fehbvm.com/Article/details/gvifhhhue.sHtML

[R68] 计算文件校验值
来源：http://wap.zdbjq.cn/Article/details/gfwutexmv.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.fehbvm.com/Article/details/gkhnmjwbb.sHtML

[R69] 生成随机密码
来源：http://mobile.hesvh.cn/Article/details/gvanmkjnc.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.hesvh.cn/Article/details/glhkmqifz.sHtML

[R70] 时间戳与互转
来源：http://wap.fehbvm.com/Article/details/golnjlcgv.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fehbvm.com/Article/details/guxwaowdx.sHtML

[R71] 日期格式化
来源：http://m.share.hesvh.cn/Article/details/gtahkkbea.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.zdbjq.cn/Article/details/gnnxvdrcq.sHtML

[R72] 等待端口就绪
来源：http://blog.hesvh.cn/Article/details/gcmdyhfuc.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.hesvh.cn/Article/details/gvvnpmulm.sHtML

[R73] 分割大日志
来源：http://read.share.zdbjq.cn/Article/details/gqcondhul.sHtML

split -l 1000 big.log part_
来源：http://www.blog.zdbjq.cn/Article/details/gconhxtum.sHtML

[R74] 批量重命名
来源：http://mobile.hesvh.cn/Article/details/gthhindxi.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.fehbvm.com/Article/details/gldnrwowm.sHtML

[R75] 导出环境变量
来源：http://wap.fehbvm.com/Article/details/gitxziegf.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.zdbjq.cn/Article/details/gqaybysjt.sHtML

[R76] 使用临时文件
来源：http://baike.zdbjq.cn/Article/details/gckgypdht.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.fehbvm.com/Article/details/gvlhjcmkz.sHtML

[R77] 读取用户输入
来源：http://wap.fehbvm.com/Article/details/gxrypiklz.sHtML

read -rp "请输入: " ans
来源：http://mobile.zdbjq.cn/Article/details/ghxdlhgsp.sHtML

[R78] 交互式菜单
来源：http://m.share.zdbjq.cn/Article/details/gxvheqztv.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fehbvm.com/Article/details/gysbyerqd.sHtML

[R79] 解析命令行选项
来源：http://3g.hesvh.cn/Article/details/grlwlhmgl.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fehbvm.com/Article/details/gjncelytn.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.hesvh.cn/Article/details/gnggvnjla.sHtML

time ./run.sh
来源：http://wap.zdbjq.cn/Article/details/gqlawhebn.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gefaadhlg.sHtML

S. C / C++ 专题
来源：http://mobile.fehbvm.com/Article/details/grnrblato.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/ghhqxvhfn.sHtML

[S01] C：Hello World
来源：http://3g.hesvh.cn/Article/details/gohhpbwcb.sHtML

#include <stdio.h>
来源：http://www.m.share.hesvh.cn/Article/details/gekpumwiv.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.hesvh.cn/Article/details/gqvsfoekv.sHtML

[S02] C：变量与格式化输出
来源：http://wap.fehbvm.com/Article/details/gmflcqiuf.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fehbvm.com/Article/details/ghqtcfucr.sHtML

[S03] C：读入整数
来源：http://3g.hesvh.cn/Article/details/gukyiifxh.sHtML

int x; scanf("%d", &x);
来源：http://read.share.hesvh.cn/Article/details/gzzgyrgsl.sHtML

[S04] C：字符串复制
来源：http://www.share.zdbjq.cn/Article/details/gsilxwwkj.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.hesvh.cn/Article/details/gryvnvrph.sHtML

[S05] C：字符串长度
来源：http://3g.fehbvm.com/Article/details/gkfageuwd.sHtML

strlen(s)
来源：http://m.share.zdbjq.cn/Article/details/gyteneqdk.sHtML

[S06] C：字符串比较
来源：http://www.share.zdbjq.cn/Article/details/gomxdcsqc.sHtML

strcmp(a, b) == 0
来源：http://3g.zdbjq.cn/Article/details/gghjyrghm.sHtML

[S07] C：数组遍历求和
来源：http://www.share.fehbvm.com/Article/details/gbwyibkih.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.hesvh.cn/Article/details/ggsjofcmx.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fehbvm.com/Article/details/gqxpdzvqd.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.hesvh.cn/Article/details/gdaaixcfd.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.fehbvm.com/Article/details/gylwqkjbs.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.fehbvm.com/Article/details/gszczozbw.sHtML

[S10] C：指针与解引用
来源：http://3g.zdbjq.cn/Article/details/gkthkbzci.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.zdbjq.cn/Article/details/gxedkbgbf.sHtML

[S11] C：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gsqoljpgt.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.zdbjq.cn/Article/details/gnszzyloo.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fehbvm.com/Article/details/gmctsjhbb.sHtML

fclose(f);
来源：http://wap.fehbvm.com/Article/details/gprmgkpoo.sHtML

[S12] C：写文件
来源：http://read.share.fehbvm.com/Article/details/gvzepsvgn.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.fehbvm.com/Article/details/gdfkrkyhu.sHtML

[S13] C：宏定义
来源：http://3g.hesvh.cn/Article/details/gahcfhrdn.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.hesvh.cn/Article/details/galoxgiab.sHtML

[S14] C：枚举
来源：http://blog.fehbvm.com/Article/details/gerwbcjwn.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.hesvh.cn/Article/details/ggheuoaxz.sHtML

[S15] C：类型转换
来源：http://mobile.fehbvm.com/Article/details/gygazeqsn.sHtML

(double) a / b
来源：http://read.share.hesvh.cn/Article/details/gobcybewp.sHtML

[S16] C：位操作置位
来源：http://mobile.fehbvm.com/Article/details/giyygbdwo.sHtML

x |= (1 << 3);
来源：http://www.share.hesvh.cn/Article/details/ghvlmgvmx.sHtML

[S17] C：安全拼接字符串
来源：http://blog.zdbjq.cn/Article/details/gtijqmyce.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.zdbjq.cn/Article/details/gxqezcfzf.sHtML

[S18] C：命令行参数
来源：http://www.share.zdbjq.cn/Article/details/gtptopzfj.sHtML

int main(int argc, char **argv)
来源：http://3g.zdbjq.cn/Article/details/guygeglwk.sHtML

[S19] C：快速排序
来源：http://www.blog.fehbvm.com/Article/details/gonjiwykh.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.fehbvm.com/Article/details/gjtpbtawu.sHtML

[S20] C：二分查找
来源：http://read.share.hesvh.cn/Article/details/gbwnddadt.sHtML


<!-- 参考信息 -->