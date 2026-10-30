代发 wailian999

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.fehbvm.com/Article/details/gcnxnvvby.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.fehbvm.com/Article/details/gbnzlhcja.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.zdbjq.cn/Article/details/ggsepwxsm.sHtML

[Q57] 行号
来源：http://www.share.hesvh.cn/Article/details/grlgpsldc.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.hesvh.cn/Article/details/gbcfqaubm.sHtML

[Q58] 累计求和
来源：http://read.share.fehbvm.com/Article/details/gkciafzqc.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/grlyjmjjt.sHtML

[Q59] 分组内累计
来源：http://m.share.hesvh.cn/Article/details/gnmnjgsug.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gfcghmhoy.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.zdbjq.cn/Article/details/gjdtkdznu.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.fehbvm.com/Article/details/gamlesokc.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.fehbvm.com/Article/details/goozhpxsm.sHtML

[Q61] 移动平均
来源：http://mobile.fehbvm.com/Article/details/gjrdiyzqm.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.fehbvm.com/Article/details/guprhhwve.sHtML

[Q62] 分组占比
来源：http://wap.zdbjq.cn/Article/details/gmqaewpfs.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/gjazcoxif.sHtML

[Q63] 开启事务
来源：http://www.blog.hesvh.cn/Article/details/gegtbqkka.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.hesvh.cn/Article/details/golfhnhpu.sHtML

[Q64] 提交事务
来源：http://www.share.hesvh.cn/Article/details/gtzgzotoi.sHtML

COMMIT;
来源：http://3g.fehbvm.com/Article/details/gmmrfjrwe.sHtML

[Q65] 回滚事务
来源：http://read.share.zdbjq.cn/Article/details/gkkkitlib.sHtML

ROLLBACK;
来源：http://www.blog.zdbjq.cn/Article/details/gehxfkikh.sHtML

[Q66] 行锁查询
来源：http://wap.fehbvm.com/Article/details/geqwhlfvi.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.hesvh.cn/Article/details/gggfcpwsn.sHtML

[Q67] 设置隔离级别
来源：http://blog.hesvh.cn/Article/details/guyvnixjz.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.fehbvm.com/Article/details/ggoearnhn.sHtML

[Q68] 保存点
来源：http://wap.fehbvm.com/Article/details/gdcjtwfrp.sHtML

SAVEPOINT sp1;
来源：http://read.share.fehbvm.com/Article/details/grijlxghr.sHtML

ROLLBACK TO sp1;
来源：http://wap.hesvh.cn/Article/details/gpcqlwsoq.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.fehbvm.com/Article/details/geeeqishh.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.hesvh.cn/Article/details/gceobalav.sHtML

[Q70] 更新统计信息
来源：http://read.share.zdbjq.cn/Article/details/gebepzekn.sHtML

ANALYZE TABLE users;
来源：http://www.blog.zdbjq.cn/Article/details/ggcgojmla.sHtML

[Q71] 查看建表语句
来源：http://read.share.fehbvm.com/Article/details/gwakdmjwt.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.fehbvm.com/Article/details/gzryhlkoe.sHtML

[Q72] 查看索引
来源：http://m.share.zdbjq.cn/Article/details/geosflvrr.sHtML

SHOW INDEX FROM users;
来源：http://3g.fehbvm.com/Article/details/glodzsnsh.sHtML

[Q73] 查看表状态
来源：http://3g.hesvh.cn/Article/details/grrdbcwaw.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.zdbjq.cn/Article/details/gfokkxlfu.sHtML

[Q74] 强制使用索引
来源：http://blog.zdbjq.cn/Article/details/gmgadsbry.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.zdbjq.cn/Article/details/gchccgtwk.sHtML

[Q75] 日期格式化
来源：http://www.share.zdbjq.cn/Article/details/gvhjgnrwv.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gfphwgtmb.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.hesvh.cn/Article/details/gyvyxvsdz.sHtML

[Q76] 按天统计
来源：http://www.m.share.fehbvm.com/Article/details/gbsoztcsu.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.zdbjq.cn/Article/details/gpoaeaqmt.sHtML

[Q77] 时间加减
来源：http://wap.zdbjq.cn/Article/details/ggevkpoue.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.hesvh.cn/Article/details/gfgpmhstv.sHtML

[Q78] 当前时间
来源：http://wap.fehbvm.com/Article/details/gtokweyda.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.zdbjq.cn/Article/details/gurpxclmu.sHtML

[Q79] 字符串拼接
来源：http://wap.hesvh.cn/Article/details/ghleggbbq.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.hesvh.cn/Article/details/gmujzzbhf.sHtML

[Q80] 字符串截取
来源：http://wap.fehbvm.com/Article/details/gcbdzgvxv.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gfxibwzxm.sHtML

[Q81] 字符串替换
来源：http://read.share.hesvh.cn/Article/details/gmqdlipes.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gwtmmblih.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.zdbjq.cn/Article/details/gwnmaftpx.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gxxsmnldc.sHtML

[Q83] 大小写转换
来源：http://baike.hesvh.cn/Article/details/gotgjblcb.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gyqoxrmnw.sHtML

[Q84] 去除首尾空格
来源：http://baike.zdbjq.cn/Article/details/gekzquawf.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/goaetuuaa.sHtML

[Q85] 数值取整
来源：http://www.share.hesvh.cn/Article/details/gfotnxoul.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.fehbvm.com/Article/details/gxiwdxmdj.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.fehbvm.com/Article/details/gbczmbgzj.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.zdbjq.cn/Article/details/gballibsu.sHtML

[Q87] JSON 字段做条件
来源：http://3g.fehbvm.com/Article/details/gtzkrgqkt.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.zdbjq.cn/Article/details/gsgvkijng.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.fehbvm.com/Article/details/gararaacv.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.hesvh.cn/Article/details/guwyofvzw.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.zdbjq.cn/Article/details/gmisdnaxe.sHtML

[Q89] 判断表是否存在
来源：http://blog.fehbvm.com/Article/details/gmgqtnfgi.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.hesvh.cn/Article/details/gsgciryly.sHtML

[Q90] 生成序号列
来源：http://blog.fehbvm.com/Article/details/gdajozgyy.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.zdbjq.cn/Article/details/gniguaiye.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gyedkbrhv.sHtML

R. Bash 专题
来源：http://www.m.share.zdbjq.cn/Article/details/gscnkxicp.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gvskcrpdt.sHtML

[R01] shebang 与严格模式
来源：http://m.share.fehbvm.com/Article/details/gstwotqdz.sHtML

#!/usr/bin/env bash
来源：http://www.share.zdbjq.cn/Article/details/gmncucfkh.sHtML

set -euo pipefail
来源：http://mobile.hesvh.cn/Article/details/gpmzniapk.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.hesvh.cn/Article/details/gdgwroddj.sHtML

name="Tom"; echo "$name"
来源：http://wap.hesvh.cn/Article/details/gmiapvxdw.sHtML

[R03] 只读变量
来源：http://baike.hesvh.cn/Article/details/gpsqldmpa.sHtML

readonly PI=3.14
来源：http://www.blog.fehbvm.com/Article/details/gqmlyxtol.sHtML

[R04] 位置参数
来源：http://read.share.fehbvm.com/Article/details/guzqjgvku.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.hesvh.cn/Article/details/gnfrkoqtv.sHtML

[R05] 参数默认值
来源：http://www.blog.hesvh.cn/Article/details/gyabzmlwx.sHtML

name="${1:-default}"
来源：http://baike.fehbvm.com/Article/details/gmxtfsnpp.sHtML

[R06] 判断命令是否存在
来源：http://mobile.fehbvm.com/Article/details/gaxonjxev.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.zdbjq.cn/Article/details/gheibvopo.sHtML

[R07] if 判断文件
来源：http://www.m.share.zdbjq.cn/Article/details/geetsngkb.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.fehbvm.com/Article/details/gpzzpigrx.sHtML

[R08] 数值比较
来源：http://baike.zdbjq.cn/Article/details/gcdnbfwzj.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.zdbjq.cn/Article/details/gevyqpxba.sHtML

[R09] 字符串比较
来源：http://3g.hesvh.cn/Article/details/grvazkmqs.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.hesvh.cn/Article/details/gwhrydalj.sHtML

[R10] 正则匹配
来源：http://baike.hesvh.cn/Article/details/glktxdtbb.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.hesvh.cn/Article/details/gkigdhqst.sHtML

[R11] case 多分支
来源：http://blog.fehbvm.com/Article/details/gucrobvhv.sHtML

case "$1" in
来源：http://www.share.zdbjq.cn/Article/details/gnkrxswjr.sHtML

start) echo "启动" ;;
来源：http://www.m.share.zdbjq.cn/Article/details/gcgfwbicj.sHtML

stop)  echo "停止" ;;
来源：http://blog.zdbjq.cn/Article/details/gbxbtqdrs.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.fehbvm.com/Article/details/gcdybgpvv.sHtML

esac
来源：http://m.share.hesvh.cn/Article/details/gytzvnrpj.sHtML

[R12] for 遍历文件
来源：http://www.m.share.hesvh.cn/Article/details/gbvuhsteq.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.hesvh.cn/Article/details/gotphdsxc.sHtML

[R13] for 计数循环
来源：http://blog.hesvh.cn/Article/details/gnqfrvgsv.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.zdbjq.cn/Article/details/gkonussss.sHtML

[R14] C 风格 for
来源：http://blog.fehbvm.com/Article/details/gikrzlxid.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.hesvh.cn/Article/details/gfohymigf.sHtML

[R15] while 逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gwlrolkxj.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gylegfrkq.sHtML

[R16] until 等待条件
来源：http://www.share.zdbjq.cn/Article/details/gdmhspcbf.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.hesvh.cn/Article/details/gsvtgsmuw.sHtML

[R17] 数组定义与取值
来源：http://www.blog.fehbvm.com/Article/details/gjcnbjere.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.hesvh.cn/Article/details/gwydgmhss.sHtML

[R18] 遍历数组
来源：http://www.share.fehbvm.com/Article/details/glrejaqco.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.zdbjq.cn/Article/details/gynehefyw.sHtML

[R19] 数组长度
来源：http://www.blog.hesvh.cn/Article/details/glcrupqcb.sHtML

echo "${#arr[@]}"
来源：http://blog.hesvh.cn/Article/details/gpwjqwxbk.sHtML

[R20] 关联数组（字典）
来源：http://blog.zdbjq.cn/Article/details/gxdmchfsr.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.zdbjq.cn/Article/details/gzncmwglp.sHtML

[R21] 字符串长度
来源：http://wap.hesvh.cn/Article/details/gnzizthqj.sHtML

echo "${#s}"
来源：http://3g.fehbvm.com/Article/details/gsuuxebph.sHtML

[R22] 截取子串
来源：http://m.share.hesvh.cn/Article/details/geiruxjua.sHtML

echo "${s:0:5}"
来源：http://read.share.fehbvm.com/Article/details/gatpgjool.sHtML

[R23] 字符串替换
来源：http://baike.zdbjq.cn/Article/details/ggkqnmpen.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.zdbjq.cn/Article/details/gchcyiang.sHtML

[R24] 大小写转换
来源：http://www.m.share.fehbvm.com/Article/details/gzkcvnyga.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.hesvh.cn/Article/details/gxwitbkpg.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.hesvh.cn/Article/details/gmphavpym.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.zdbjq.cn/Article/details/gbfbzkqlq.sHtML

[R26] 命令替换
来源：http://wap.hesvh.cn/Article/details/gxzlykmbc.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.fehbvm.com/Article/details/gdarvbqqv.sHtML

[R27] 算术展开
来源：http://read.share.hesvh.cn/Article/details/gbdptxxsn.sHtML

echo $((1 + 2 * 3))
来源：http://wap.hesvh.cn/Article/details/gbgbwbgsk.sHtML

[R28] 浮点运算
来源：http://wap.fehbvm.com/Article/details/gynecdzak.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.fehbvm.com/Article/details/gxsayysly.sHtML

[R29] 定义函数
来源：http://blog.hesvh.cn/Article/details/gcywbgwgh.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.fehbvm.com/Article/details/gbpqjoied.sHtML

[R30] 函数返回状态码
来源：http://read.share.hesvh.cn/Article/details/gzrndwexw.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.fehbvm.com/Article/details/gtfkaxgvh.sHtML

[R31] 局部变量
来源：http://www.m.share.zdbjq.cn/Article/details/ghdsgnoym.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.fehbvm.com/Article/details/guetqjbrl.sHtML

[R32] 参数个数校验
来源：http://blog.fehbvm.com/Article/details/gziaqrajj.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.zdbjq.cn/Article/details/gqsgjessu.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fehbvm.com/Article/details/gpqdnbikj.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.hesvh.cn/Article/details/grvylesbw.sHtML

[R34] 退出时清理
来源：http://read.share.fehbvm.com/Article/details/gyainxafd.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fehbvm.com/Article/details/gjsztmgdw.sHtML

[R35] 后台执行并等待
来源：http://baike.fehbvm.com/Article/details/gpnaesefd.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.fehbvm.com/Article/details/gonmwkslf.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fehbvm.com/Article/details/gyadbnebr.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.zdbjq.cn/Article/details/gptzfqbrv.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.hesvh.cn/Article/details/glbofjpnd.sHtML

files=$(ls -1)
来源：http://blog.zdbjq.cn/Article/details/gutxumqte.sHtML

[R38] 管道串联
来源：http://mobile.zdbjq.cn/Article/details/gwsnddbpr.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.hesvh.cn/Article/details/gizgypraz.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.hesvh.cn/Article/details/gacjdojwr.sHtML

cmd > out.log 2>&1
来源：http://wap.hesvh.cn/Article/details/gmeffiizx.sHtML

[R40] 追加写日志
来源：http://m.share.fehbvm.com/Article/details/gqyormlpc.sHtML

echo "log" >> out.log
来源：http://mobile.fehbvm.com/Article/details/goccqdjgk.sHtML

[R41] 丢弃输出
来源：http://mobile.fehbvm.com/Article/details/gzeitcgmv.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fehbvm.com/Article/details/gfxkeeyhp.sHtML

[R42] 输入重定向
来源：http://m.share.hesvh.cn/Article/details/ggoctglvg.sHtML

wc -l < a.txt
来源：http://www.share.hesvh.cn/Article/details/gdofhdsrr.sHtML

[R43] 按名字查找文件
来源：http://m.share.hesvh.cn/Article/details/gleazybwb.sHtML

find . -name "*.log" -type f
来源：http://read.share.fehbvm.com/Article/details/gdupullmf.sHtML

[R44] 按修改时间查找
来源：http://blog.hesvh.cn/Article/details/gqffkywdv.sHtML

find . -mtime -7 -type f
来源：http://www.share.fehbvm.com/Article/details/gxsiwrzwn.sHtML

[R45] 批量删除
来源：http://www.share.hesvh.cn/Article/details/gyazjilza.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.hesvh.cn/Article/details/gyefijtxd.sHtML

[R46] 递归替换文件内容
来源：http://baike.hesvh.cn/Article/details/gukwpzbqt.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.zdbjq.cn/Article/details/gkfftdygl.sHtML

[R47] sed 单行替换
来源：http://m.share.hesvh.cn/Article/details/gfqtjkulb.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.zdbjq.cn/Article/details/goiaubkiz.sHtML

[R48] awk 取指定列
来源：http://baike.fehbvm.com/Article/details/gnkrenulg.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.zdbjq.cn/Article/details/gcgkuaikw.sHtML

[R49] awk 带条件
来源：http://read.share.hesvh.cn/Article/details/gvbgwxqyb.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fehbvm.com/Article/details/gzzajalwb.sHtML

[R50] awk 求和
来源：http://3g.hesvh.cn/Article/details/gtuciokgq.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.hesvh.cn/Article/details/gectpiubl.sHtML

[R51] 排序去重取前几
来源：http://mobile.hesvh.cn/Article/details/ghjollggj.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.fehbvm.com/Article/details/gvehdpqgh.sHtML

[R52] 统计行数
来源：http://wap.fehbvm.com/Article/details/gwhibihzi.sHtML

wc -l a.txt
来源：http://baike.hesvh.cn/Article/details/gixenzoyn.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.hesvh.cn/Article/details/glqicmvea.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.hesvh.cn/Article/details/gxjhiuhcg.sHtML

[R54] 比较两个文件
来源：http://baike.fehbvm.com/Article/details/ggvmydhjw.sHtML

diff a.txt b.txt
来源：http://3g.hesvh.cn/Article/details/gyuptzqap.sHtML

[R55] 压缩与解压
来源：http://www.m.share.fehbvm.com/Article/details/gnhcjgrpy.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fehbvm.com/Article/details/grjflhdcr.sHtML

[R56] 远程拷贝
来源：http://mobile.fehbvm.com/Article/details/gdqbakcgb.sHtML

scp file user@host:/path/
来源：http://wap.fehbvm.com/Article/details/gdqitwxfw.sHtML

[R57] 远程执行命令
来源：http://www.m.share.hesvh.cn/Article/details/gtecaklwn.sHtML

ssh user@host 'uptime'
来源：http://blog.zdbjq.cn/Article/details/gimtfzzzk.sHtML

[R58] 下载文件
来源：http://www.share.zdbjq.cn/Article/details/gzvzkncnj.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.zdbjq.cn/Article/details/gjtveipcu.sHtML

[R59] 发 POST JSON
来源：http://baike.zdbjq.cn/Article/details/grmfyewun.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fehbvm.com/Article/details/glkrgcgnn.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.zdbjq.cn/Article/details/gsranctkv.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.fehbvm.com/Article/details/guxbaczzo.sHtML

[R61] 磁盘占用
来源：http://read.share.hesvh.cn/Article/details/gspqyqlgm.sHtML

df -h;  du -sh *
来源：http://baike.hesvh.cn/Article/details/ggljlowbq.sHtML

[R62] 找最占空间的文件
来源：http://m.share.zdbjq.cn/Article/details/geuenflha.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.zdbjq.cn/Article/details/gzdfpvmsa.sHtML

[R63] 内存与进程
来源：http://wap.hesvh.cn/Article/details/gsmjfhitu.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.hesvh.cn/Article/details/gufkpvwzz.sHtML

[R64] 结束进程
来源：http://blog.fehbvm.com/Article/details/gpugbwzjg.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fehbvm.com/Article/details/gsncgutcv.sHtML

[R65] 查看端口占用
来源：http://wap.zdbjq.cn/Article/details/gpbqoxbcf.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.fehbvm.com/Article/details/gtxkfljbb.sHtML

[R66] 定时任务
来源：http://www.share.fehbvm.com/Article/details/gmnmtuufc.sHtML

crontab -e;  crontab -l
来源：http://wap.hesvh.cn/Article/details/gawbzvhjf.sHtML

[R67] 生成随机十六进制串
来源：http://3g.hesvh.cn/Article/details/gzsqiloki.sHtML

openssl rand -hex 16
来源：http://m.share.zdbjq.cn/Article/details/guidfurpt.sHtML

[R68] 计算文件校验值
来源：http://blog.zdbjq.cn/Article/details/gonkmdzob.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.zdbjq.cn/Article/details/ghtwrcszu.sHtML

[R69] 生成随机密码
来源：http://baike.fehbvm.com/Article/details/gjluzitxd.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fehbvm.com/Article/details/gspkvwonr.sHtML

[R70] 时间戳与互转
来源：http://3g.zdbjq.cn/Article/details/gzuwqawra.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.hesvh.cn/Article/details/gyncpgahs.sHtML

[R71] 日期格式化
来源：http://www.share.hesvh.cn/Article/details/gxqtzkqmi.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.fehbvm.com/Article/details/gjvffdsvs.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.zdbjq.cn/Article/details/geoqjsoyw.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fehbvm.com/Article/details/gqslglkrt.sHtML

[R73] 分割大日志
来源：http://mobile.zdbjq.cn/Article/details/gpsjcoaqc.sHtML

split -l 1000 big.log part_
来源：http://3g.fehbvm.com/Article/details/gyumlpuyu.sHtML

[R74] 批量重命名
来源：http://read.share.hesvh.cn/Article/details/geilkhtnx.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.hesvh.cn/Article/details/gfvzppobt.sHtML

[R75] 导出环境变量
来源：http://mobile.zdbjq.cn/Article/details/girgqcwav.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.zdbjq.cn/Article/details/gezcsmqbt.sHtML

[R76] 使用临时文件
来源：http://read.share.fehbvm.com/Article/details/gzrjrkznz.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.hesvh.cn/Article/details/gamvlxstd.sHtML

[R77] 读取用户输入
来源：http://www.share.hesvh.cn/Article/details/gpxjlgmpa.sHtML

read -rp "请输入: " ans
来源：http://mobile.hesvh.cn/Article/details/gbyfepzki.sHtML

[R78] 交互式菜单
来源：http://wap.zdbjq.cn/Article/details/gzbhcmgoa.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.zdbjq.cn/Article/details/ggfyjnrjt.sHtML

[R79] 解析命令行选项
来源：http://www.blog.zdbjq.cn/Article/details/gpplunolp.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.fehbvm.com/Article/details/gntfacgvm.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.fehbvm.com/Article/details/gghppvgsg.sHtML

time ./run.sh
来源：http://baike.fehbvm.com/Article/details/gesqyqdxx.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gxsbybdhz.sHtML

S. C / C++ 专题
来源：http://blog.fehbvm.com/Article/details/gjjdhrjlu.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gpjpepsbs.sHtML

[S01] C：Hello World
来源：http://blog.fehbvm.com/Article/details/gzfbmkxxj.sHtML

#include <stdio.h>
来源：http://blog.fehbvm.com/Article/details/gkakgjtbi.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.fehbvm.com/Article/details/gbnrutbkq.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.fehbvm.com/Article/details/ghnobykpi.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.zdbjq.cn/Article/details/gmdcyoijr.sHtML

[S03] C：读入整数
来源：http://blog.zdbjq.cn/Article/details/gbowsynwq.sHtML

int x; scanf("%d", &x);
来源：http://blog.zdbjq.cn/Article/details/gpyrhskui.sHtML

[S04] C：字符串复制
来源：http://3g.fehbvm.com/Article/details/ghvbauvte.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.hesvh.cn/Article/details/ghfhifrqa.sHtML

[S05] C：字符串长度
来源：http://www.blog.hesvh.cn/Article/details/gbsqtnpgl.sHtML

strlen(s)
来源：http://blog.zdbjq.cn/Article/details/gcwmktqqh.sHtML

[S06] C：字符串比较
来源：http://blog.fehbvm.com/Article/details/grwlcsvil.sHtML

strcmp(a, b) == 0
来源：http://read.share.zdbjq.cn/Article/details/gvxojdgsc.sHtML

[S07] C：数组遍历求和
来源：http://3g.fehbvm.com/Article/details/gwthomtyz.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.zdbjq.cn/Article/details/gphuucwhy.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.zdbjq.cn/Article/details/gdzdbwhnq.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.zdbjq.cn/Article/details/gnuexetwf.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.hesvh.cn/Article/details/gidbrotwh.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fehbvm.com/Article/details/gleiguyjp.sHtML

[S10] C：指针与解引用
来源：http://baike.zdbjq.cn/Article/details/gwtaisffi.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.zdbjq.cn/Article/details/gxptbmdei.sHtML

[S11] C：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gacodxesg.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fehbvm.com/Article/details/gewrofenq.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.hesvh.cn/Article/details/girshshwv.sHtML

fclose(f);
来源：http://mobile.fehbvm.com/Article/details/gshshfwjt.sHtML

[S12] C：写文件
来源：http://www.m.share.hesvh.cn/Article/details/gksoqaoys.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.zdbjq.cn/Article/details/grochqdeb.sHtML

[S13] C：宏定义
来源：http://www.m.share.hesvh.cn/Article/details/glpbynyzj.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fehbvm.com/Article/details/gbvxhplgh.sHtML

[S14] C：枚举
来源：http://www.m.share.fehbvm.com/Article/details/gzagiinap.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.hesvh.cn/Article/details/ghdqwqpbb.sHtML

[S15] C：类型转换
来源：http://blog.fehbvm.com/Article/details/gkilmgnbl.sHtML

(double) a / b
来源：http://mobile.hesvh.cn/Article/details/gcokzrlrn.sHtML

[S16] C：位操作置位
来源：http://www.share.zdbjq.cn/Article/details/gdqjrdtjy.sHtML

x |= (1 << 3);
来源：http://mobile.zdbjq.cn/Article/details/geacryjaq.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/glddkecxo.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.fehbvm.com/Article/details/gkpmzaxwv.sHtML

[S18] C：命令行参数
来源：http://www.share.fehbvm.com/Article/details/ggcwouhfg.sHtML

int main(int argc, char **argv)
来源：http://baike.zdbjq.cn/Article/details/gingxqmka.sHtML

[S19] C：快速排序
来源：http://www.share.zdbjq.cn/Article/details/gyygpggwc.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fehbvm.com/Article/details/gbjvrfwpd.sHtML

[S20] C：二分查找
来源：http://3g.fehbvm.com/Article/details/gvmvzhymx.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.hesvh.cn/Article/details/gfkivchka.sHtML

[S21] C：字符类别判断
来源：http://mobile.zdbjq.cn/Article/details/goscwxgsu.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.zdbjq.cn/Article/details/gcyzyisgc.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fehbvm.com/Article/details/goptksodq.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.hesvh.cn/Article/details/gctkgdwpn.sHtML

[S23] C：随机数
来源：http://www.m.share.zdbjq.cn/Article/details/gfsjmbnqg.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.hesvh.cn/Article/details/gknbmerzj.sHtML

[S24] C：获取本地时间
来源：http://wap.fehbvm.com/Article/details/gkqptsvkn.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.hesvh.cn/Article/details/grxsxnsjn.sHtML

[S25] C：内存拷贝
来源：http://www.blog.hesvh.cn/Article/details/gqtwldppq.sHtML

memcpy(dst, src, n);
来源：http://wap.zdbjq.cn/Article/details/gdopcwpjy.sHtML

[S26] C：内存清零
来源：http://m.share.hesvh.cn/Article/details/gmqkiqfzy.sHtML


<!-- 参考信息 -->