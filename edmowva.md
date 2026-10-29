代发 wailian999

ROLLBACK TO sp1;
来源：http://www.m.share.zdbjq.cn/Article/details/gtuhmlebd.sHtML

[Q69] 查看执行计划
来源：http://baike.fehbvm.com/Article/details/gpwgnxglu.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.zdbjq.cn/Article/details/gwuymxyfq.sHtML

[Q70] 更新统计信息
来源：http://read.share.fehbvm.com/Article/details/gkingeoob.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.zdbjq.cn/Article/details/gkfwygnii.sHtML

[Q71] 查看建表语句
来源：http://mobile.hesvh.cn/Article/details/gfneifjrw.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.hesvh.cn/Article/details/gajtvzlgm.sHtML

[Q72] 查看索引
来源：http://m.share.fehbvm.com/Article/details/gjybtmzzm.sHtML

SHOW INDEX FROM users;
来源：http://wap.hesvh.cn/Article/details/gbpebpffy.sHtML

[Q73] 查看表状态
来源：http://mobile.hesvh.cn/Article/details/gqgopudft.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.zdbjq.cn/Article/details/gbmvsmwzq.sHtML

[Q74] 强制使用索引
来源：http://wap.zdbjq.cn/Article/details/gjjeowvyh.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.fehbvm.com/Article/details/gsvvgvmue.sHtML

[Q75] 日期格式化
来源：http://blog.fehbvm.com/Article/details/gextkwrkc.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gfhbphtmz.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.hesvh.cn/Article/details/gujflxxkj.sHtML

[Q76] 按天统计
来源：http://wap.zdbjq.cn/Article/details/gfxhonkxj.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.fehbvm.com/Article/details/gggvxcsvv.sHtML

[Q77] 时间加减
来源：http://www.share.fehbvm.com/Article/details/gfociissw.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.zdbjq.cn/Article/details/gzpnsqzvx.sHtML

[Q78] 当前时间
来源：http://baike.fehbvm.com/Article/details/gpzzqtzlb.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.fehbvm.com/Article/details/glythvbtd.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.zdbjq.cn/Article/details/gybmtyjxx.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.hesvh.cn/Article/details/gpmxbdrag.sHtML

[Q80] 字符串截取
来源：http://m.share.hesvh.cn/Article/details/gukyxewqa.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gxjxehvyj.sHtML

[Q81] 字符串替换
来源：http://baike.zdbjq.cn/Article/details/gzdrfqqym.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.fehbvm.com/Article/details/gbprctajh.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.hesvh.cn/Article/details/gjopxzjmj.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gironihwc.sHtML

[Q83] 大小写转换
来源：http://www.blog.hesvh.cn/Article/details/gievvzpuf.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gvwwwdlex.sHtML

[Q84] 去除首尾空格
来源：http://3g.hesvh.cn/Article/details/gewvkdcnh.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/ggitdelzw.sHtML

[Q85] 数值取整
来源：http://wap.fehbvm.com/Article/details/gwwvfrppf.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.zdbjq.cn/Article/details/grnkzdjom.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.fehbvm.com/Article/details/gijlhzpog.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.fehbvm.com/Article/details/gsmibrjri.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.zdbjq.cn/Article/details/giffsunsb.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.zdbjq.cn/Article/details/gnibgziwc.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.hesvh.cn/Article/details/gbzibiqaj.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.fehbvm.com/Article/details/gysceciky.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.zdbjq.cn/Article/details/glrtfdpso.sHtML

[Q89] 判断表是否存在
来源：http://blog.hesvh.cn/Article/details/gkeloilkb.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.fehbvm.com/Article/details/gzjwqrnfg.sHtML

[Q90] 生成序号列
来源：http://wap.zdbjq.cn/Article/details/glvbahkqk.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.zdbjq.cn/Article/details/gotncpjaw.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gdndbybxq.sHtML

R. Bash 专题
来源：http://www.blog.hesvh.cn/Article/details/gsciybjfo.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gdlhvrxrs.sHtML

[R01] shebang 与严格模式
来源：http://3g.fehbvm.com/Article/details/gvwjbeuqi.sHtML

#!/usr/bin/env bash
来源：http://mobile.fehbvm.com/Article/details/gnxrrdjfx.sHtML

set -euo pipefail
来源：http://blog.zdbjq.cn/Article/details/gipoaguvp.sHtML

[R02] 变量赋值与使用
来源：http://baike.hesvh.cn/Article/details/gkftoklvh.sHtML

name="Tom"; echo "$name"
来源：http://wap.hesvh.cn/Article/details/gqtncobgm.sHtML

[R03] 只读变量
来源：http://m.share.fehbvm.com/Article/details/guzdbzpcw.sHtML

readonly PI=3.14
来源：http://mobile.fehbvm.com/Article/details/guhgfaudc.sHtML

[R04] 位置参数
来源：http://read.share.zdbjq.cn/Article/details/glcqxqzkd.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.fehbvm.com/Article/details/gfqpmplrz.sHtML

[R05] 参数默认值
来源：http://www.blog.fehbvm.com/Article/details/geuylthsr.sHtML

name="${1:-default}"
来源：http://mobile.hesvh.cn/Article/details/gumqsggoi.sHtML

[R06] 判断命令是否存在
来源：http://baike.zdbjq.cn/Article/details/gqxvmkbgh.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fehbvm.com/Article/details/gliaqclgj.sHtML

[R07] if 判断文件
来源：http://www.share.hesvh.cn/Article/details/gfafhvmcp.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.zdbjq.cn/Article/details/gzmtetrau.sHtML

[R08] 数值比较
来源：http://www.m.share.zdbjq.cn/Article/details/glqhexcse.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.zdbjq.cn/Article/details/gavwkarso.sHtML

[R09] 字符串比较
来源：http://3g.fehbvm.com/Article/details/gydvpxtic.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.hesvh.cn/Article/details/gwwvhphmh.sHtML

[R10] 正则匹配
来源：http://m.share.hesvh.cn/Article/details/gowkwcicw.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.hesvh.cn/Article/details/gfnplgtdb.sHtML

[R11] case 多分支
来源：http://m.share.zdbjq.cn/Article/details/gyvqsxixv.sHtML

case "$1" in
来源：http://www.blog.zdbjq.cn/Article/details/gnqxrcpdw.sHtML

start) echo "启动" ;;
来源：http://read.share.hesvh.cn/Article/details/gmeffroxu.sHtML

stop)  echo "停止" ;;
来源：http://m.share.zdbjq.cn/Article/details/gjxbvtxdx.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.hesvh.cn/Article/details/gcxgcoswv.sHtML

esac
来源：http://blog.hesvh.cn/Article/details/gglusedci.sHtML

[R12] for 遍历文件
来源：http://www.share.zdbjq.cn/Article/details/gojqyphzn.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.fehbvm.com/Article/details/gewspgoms.sHtML

[R13] for 计数循环
来源：http://www.share.zdbjq.cn/Article/details/gbjtrqrgw.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.zdbjq.cn/Article/details/gyqmcfitz.sHtML

[R14] C 风格 for
来源：http://m.share.fehbvm.com/Article/details/gdfofvlty.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.fehbvm.com/Article/details/gngdurxkc.sHtML

[R15] while 逐行读文件
来源：http://3g.hesvh.cn/Article/details/ggsiltdcf.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.hesvh.cn/Article/details/gwdfyubok.sHtML

[R16] until 等待条件
来源：http://blog.hesvh.cn/Article/details/gepzztxfc.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.hesvh.cn/Article/details/gxffvobvx.sHtML

[R17] 数组定义与取值
来源：http://www.share.hesvh.cn/Article/details/gfgponyjm.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.hesvh.cn/Article/details/gddophdqj.sHtML

[R18] 遍历数组
来源：http://read.share.fehbvm.com/Article/details/gdmgirfej.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.zdbjq.cn/Article/details/gjnczuwcn.sHtML

[R19] 数组长度
来源：http://blog.zdbjq.cn/Article/details/gdtylxogb.sHtML

echo "${#arr[@]}"
来源：http://read.share.zdbjq.cn/Article/details/glwaxgrfe.sHtML

[R20] 关联数组（字典）
来源：http://read.share.hesvh.cn/Article/details/gxaulvfzo.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.zdbjq.cn/Article/details/gzslffqpn.sHtML

[R21] 字符串长度
来源：http://blog.fehbvm.com/Article/details/gmejnwfrm.sHtML

echo "${#s}"
来源：http://mobile.zdbjq.cn/Article/details/gptgifzon.sHtML

[R22] 截取子串
来源：http://www.blog.hesvh.cn/Article/details/gbiwezmyz.sHtML

echo "${s:0:5}"
来源：http://www.m.share.hesvh.cn/Article/details/gfwnxxhbt.sHtML

[R23] 字符串替换
来源：http://blog.fehbvm.com/Article/details/grvsvnmlc.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.fehbvm.com/Article/details/gxuqssoza.sHtML

[R24] 大小写转换
来源：http://baike.zdbjq.cn/Article/details/gtsnpgnkt.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.fehbvm.com/Article/details/gvzjrqtcj.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.hesvh.cn/Article/details/ghwfbsnfv.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.fehbvm.com/Article/details/gvscppphz.sHtML

[R26] 命令替换
来源：http://www.blog.hesvh.cn/Article/details/gdyaukyab.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.zdbjq.cn/Article/details/gnqvgszve.sHtML

[R27] 算术展开
来源：http://3g.hesvh.cn/Article/details/gitrvsrrn.sHtML

echo $((1 + 2 * 3))
来源：http://blog.fehbvm.com/Article/details/gpkflvkgf.sHtML

[R28] 浮点运算
来源：http://blog.hesvh.cn/Article/details/guzbypprm.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.zdbjq.cn/Article/details/gszyhuvzy.sHtML

[R29] 定义函数
来源：http://baike.hesvh.cn/Article/details/gjjzlstke.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.zdbjq.cn/Article/details/gdpelqzbd.sHtML

[R30] 函数返回状态码
来源：http://www.blog.zdbjq.cn/Article/details/gkuaavwhl.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.hesvh.cn/Article/details/gjluwohut.sHtML

[R31] 局部变量
来源：http://3g.zdbjq.cn/Article/details/gcfbjiugl.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.hesvh.cn/Article/details/ggfldbwjo.sHtML

[R32] 参数个数校验
来源：http://m.share.hesvh.cn/Article/details/gspwaqxoa.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.zdbjq.cn/Article/details/gooqtssvh.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.zdbjq.cn/Article/details/ghgxfgpji.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.hesvh.cn/Article/details/gbatxmjvc.sHtML

[R34] 退出时清理
来源：http://m.share.zdbjq.cn/Article/details/gkvydolmf.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.hesvh.cn/Article/details/gpginpvlt.sHtML

[R35] 后台执行并等待
来源：http://mobile.fehbvm.com/Article/details/genewkobf.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.zdbjq.cn/Article/details/ggeodirxd.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.fehbvm.com/Article/details/gdlrchkqa.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.fehbvm.com/Article/details/grpytkhhb.sHtML

[R37] 把输出赋给变量
来源：http://read.share.zdbjq.cn/Article/details/gteyzrjde.sHtML

files=$(ls -1)
来源：http://baike.zdbjq.cn/Article/details/gswlsvdml.sHtML

[R38] 管道串联
来源：http://baike.fehbvm.com/Article/details/gjeyhesko.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.fehbvm.com/Article/details/gkbrkphxc.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.hesvh.cn/Article/details/gsmtomctj.sHtML

cmd > out.log 2>&1
来源：http://blog.zdbjq.cn/Article/details/gxbddgwss.sHtML

[R40] 追加写日志
来源：http://m.share.hesvh.cn/Article/details/gvgttwojr.sHtML

echo "log" >> out.log
来源：http://m.share.zdbjq.cn/Article/details/gbultkrsa.sHtML

[R41] 丢弃输出
来源：http://www.blog.hesvh.cn/Article/details/gepkxinwa.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.zdbjq.cn/Article/details/gqzkhtayw.sHtML

[R42] 输入重定向
来源：http://mobile.zdbjq.cn/Article/details/golggcsak.sHtML

wc -l < a.txt
来源：http://blog.hesvh.cn/Article/details/gjtmgeakr.sHtML

[R43] 按名字查找文件
来源：http://www.share.fehbvm.com/Article/details/gjhgpltmq.sHtML

find . -name "*.log" -type f
来源：http://wap.zdbjq.cn/Article/details/guehbtrdr.sHtML

[R44] 按修改时间查找
来源：http://read.share.zdbjq.cn/Article/details/glsjxdane.sHtML

find . -mtime -7 -type f
来源：http://baike.zdbjq.cn/Article/details/gqfhgpqpf.sHtML

[R45] 批量删除
来源：http://blog.zdbjq.cn/Article/details/gvziejcnr.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.fehbvm.com/Article/details/glekdrdwv.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.hesvh.cn/Article/details/gkhdqdmaf.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.zdbjq.cn/Article/details/goggysilk.sHtML

[R47] sed 单行替换
来源：http://wap.fehbvm.com/Article/details/gvbsjgumr.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.zdbjq.cn/Article/details/ginzklqgt.sHtML

[R48] awk 取指定列
来源：http://blog.hesvh.cn/Article/details/gkmwicfbn.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.fehbvm.com/Article/details/gpqjvgdci.sHtML

[R49] awk 带条件
来源：http://m.share.hesvh.cn/Article/details/gfwmaeerc.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.fehbvm.com/Article/details/gytixjpgc.sHtML

[R50] awk 求和
来源：http://www.blog.hesvh.cn/Article/details/gauennjws.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.hesvh.cn/Article/details/gepzkdwmr.sHtML

[R51] 排序去重取前几
来源：http://m.share.fehbvm.com/Article/details/gtlevwlsf.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.zdbjq.cn/Article/details/gkhbatrpe.sHtML

[R52] 统计行数
来源：http://wap.hesvh.cn/Article/details/gzzewxabt.sHtML

wc -l a.txt
来源：http://m.share.hesvh.cn/Article/details/gmnclzcgd.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.zdbjq.cn/Article/details/gzlsvaluh.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.fehbvm.com/Article/details/gvrphkdcf.sHtML

[R54] 比较两个文件
来源：http://wap.fehbvm.com/Article/details/gttlkumtw.sHtML

diff a.txt b.txt
来源：http://mobile.zdbjq.cn/Article/details/gpkvguvvn.sHtML

[R55] 压缩与解压
来源：http://blog.hesvh.cn/Article/details/gxrwaltdv.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.hesvh.cn/Article/details/ghrrwoxtc.sHtML

[R56] 远程拷贝
来源：http://baike.zdbjq.cn/Article/details/gdejixkxe.sHtML

scp file user@host:/path/
来源：http://www.m.share.zdbjq.cn/Article/details/ggvmdocuw.sHtML

[R57] 远程执行命令
来源：http://blog.zdbjq.cn/Article/details/gnpsgpwog.sHtML

ssh user@host 'uptime'
来源：http://www.share.fehbvm.com/Article/details/gnjjsvcku.sHtML

[R58] 下载文件
来源：http://3g.hesvh.cn/Article/details/gvrfvjczz.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.fehbvm.com/Article/details/gvmykpqqd.sHtML

[R59] 发 POST JSON
来源：http://read.share.zdbjq.cn/Article/details/giwrnmvaa.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.zdbjq.cn/Article/details/gvudbhulb.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.zdbjq.cn/Article/details/gqzsrgvxl.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.zdbjq.cn/Article/details/gytbiadye.sHtML

[R61] 磁盘占用
来源：http://mobile.hesvh.cn/Article/details/gwoodxsja.sHtML

df -h;  du -sh *
来源：http://www.blog.fehbvm.com/Article/details/gegaeuwuw.sHtML

[R62] 找最占空间的文件
来源：http://wap.fehbvm.com/Article/details/gjocbhzas.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.hesvh.cn/Article/details/gxktiqiyn.sHtML

[R63] 内存与进程
来源：http://read.share.zdbjq.cn/Article/details/gtebunkxv.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.fehbvm.com/Article/details/gkomupmns.sHtML

[R64] 结束进程
来源：http://baike.hesvh.cn/Article/details/gunbcbdda.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.hesvh.cn/Article/details/gbbuxrtlp.sHtML

[R65] 查看端口占用
来源：http://baike.hesvh.cn/Article/details/gxqecqssb.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.zdbjq.cn/Article/details/gvyawjjcv.sHtML

[R66] 定时任务
来源：http://www.m.share.zdbjq.cn/Article/details/gmccazdnq.sHtML

crontab -e;  crontab -l
来源：http://www.share.fehbvm.com/Article/details/gzidtlntf.sHtML

[R67] 生成随机十六进制串
来源：http://blog.zdbjq.cn/Article/details/gqapoiagb.sHtML

openssl rand -hex 16
来源：http://wap.hesvh.cn/Article/details/gyrslmivo.sHtML

[R68] 计算文件校验值
来源：http://www.blog.hesvh.cn/Article/details/gdkgxkdmw.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.zdbjq.cn/Article/details/gtovbbdbr.sHtML

[R69] 生成随机密码
来源：http://wap.fehbvm.com/Article/details/gzyobhhvh.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.fehbvm.com/Article/details/gholvdyuo.sHtML

[R70] 时间戳与互转
来源：http://www.share.fehbvm.com/Article/details/ghnfqoejs.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fehbvm.com/Article/details/gtftcwjzf.sHtML

[R71] 日期格式化
来源：http://www.blog.hesvh.cn/Article/details/ghoighgol.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fehbvm.com/Article/details/gwzoqpnlu.sHtML

[R72] 等待端口就绪
来源：http://read.share.fehbvm.com/Article/details/gkpiwbrem.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.fehbvm.com/Article/details/gexpxnzkb.sHtML

[R73] 分割大日志
来源：http://read.share.hesvh.cn/Article/details/gkjjjyazl.sHtML

split -l 1000 big.log part_
来源：http://m.share.zdbjq.cn/Article/details/gvpmyefjw.sHtML

[R74] 批量重命名
来源：http://3g.fehbvm.com/Article/details/gttrsttwy.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.fehbvm.com/Article/details/gpizueuqi.sHtML

[R75] 导出环境变量
来源：http://read.share.fehbvm.com/Article/details/gcpxmrukc.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.hesvh.cn/Article/details/gqftquylk.sHtML

[R76] 使用临时文件
来源：http://www.m.share.fehbvm.com/Article/details/gtrtvgrqf.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.hesvh.cn/Article/details/gotezghyo.sHtML

[R77] 读取用户输入
来源：http://www.m.share.zdbjq.cn/Article/details/gdjkycqqk.sHtML

read -rp "请输入: " ans
来源：http://www.blog.zdbjq.cn/Article/details/gpfjyvgau.sHtML

[R78] 交互式菜单
来源：http://www.m.share.fehbvm.com/Article/details/grdhlttvi.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.fehbvm.com/Article/details/grsgrvucc.sHtML

[R79] 解析命令行选项
来源：http://read.share.hesvh.cn/Article/details/gebfccxnz.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.zdbjq.cn/Article/details/girhyhyhi.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.fehbvm.com/Article/details/gutzzflgx.sHtML

time ./run.sh
来源：http://www.m.share.hesvh.cn/Article/details/glkrsgzby.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gbamuruio.sHtML

S. C / C++ 专题
来源：http://m.share.zdbjq.cn/Article/details/gkowaztgx.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gbevotjvy.sHtML

[S01] C：Hello World
来源：http://3g.hesvh.cn/Article/details/gnmfdrhrw.sHtML

#include <stdio.h>
来源：http://read.share.hesvh.cn/Article/details/gbnmcytpb.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.zdbjq.cn/Article/details/gfrskunyo.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fehbvm.com/Article/details/gtlmmruhv.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fehbvm.com/Article/details/gcumkuenk.sHtML

[S03] C：读入整数
来源：http://www.blog.fehbvm.com/Article/details/gtvegqyow.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.hesvh.cn/Article/details/gpdzilque.sHtML

[S04] C：字符串复制
来源：http://3g.hesvh.cn/Article/details/gfueynljn.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.zdbjq.cn/Article/details/gukzrdgdy.sHtML

[S05] C：字符串长度
来源：http://3g.zdbjq.cn/Article/details/ghnuheyju.sHtML

strlen(s)
来源：http://m.share.fehbvm.com/Article/details/gubjgcayh.sHtML

[S06] C：字符串比较
来源：http://mobile.zdbjq.cn/Article/details/gcyxvfpze.sHtML

strcmp(a, b) == 0
来源：http://read.share.hesvh.cn/Article/details/gshxgyesu.sHtML

[S07] C：数组遍历求和
来源：http://read.share.hesvh.cn/Article/details/gxggsrjfc.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.fehbvm.com/Article/details/gaaceduqd.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.zdbjq.cn/Article/details/ghiqqzple.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.hesvh.cn/Article/details/grpwettqb.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.fehbvm.com/Article/details/grlsmsnwd.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.zdbjq.cn/Article/details/gwmnpneud.sHtML

[S10] C：指针与解引用
来源：http://read.share.fehbvm.com/Article/details/gguuiwzal.sHtML

int *p = &a;  *p = 5;
来源：http://blog.zdbjq.cn/Article/details/ghpwnyizd.sHtML

[S11] C：逐行读文件
来源：http://wap.hesvh.cn/Article/details/guwjgwtpl.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fehbvm.com/Article/details/gylirzngl.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fehbvm.com/Article/details/glnmcqmcq.sHtML

fclose(f);
来源：http://www.m.share.fehbvm.com/Article/details/gqllmpqkx.sHtML

[S12] C：写文件
来源：http://3g.zdbjq.cn/Article/details/ggcsdeenu.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.fehbvm.com/Article/details/grrbbpckf.sHtML

[S13] C：宏定义
来源：http://baike.zdbjq.cn/Article/details/ghevmfbbs.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.hesvh.cn/Article/details/glwzjcwbp.sHtML

[S14] C：枚举
来源：http://www.m.share.zdbjq.cn/Article/details/groeuzgnp.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.zdbjq.cn/Article/details/gnjnnoqho.sHtML

[S15] C：类型转换
来源：http://m.share.hesvh.cn/Article/details/gytbkjphb.sHtML

(double) a / b
来源：http://m.share.zdbjq.cn/Article/details/guhedquwy.sHtML

[S16] C：位操作置位
来源：http://www.blog.hesvh.cn/Article/details/gsvepdkju.sHtML

x |= (1 << 3);
来源：http://www.share.fehbvm.com/Article/details/gxhnjonrs.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/gomakvmnd.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.hesvh.cn/Article/details/ghpnbqasl.sHtML

[S18] C：命令行参数
来源：http://blog.fehbvm.com/Article/details/gvhkmmpoi.sHtML

int main(int argc, char **argv)
来源：http://read.share.zdbjq.cn/Article/details/gnhofgenh.sHtML

[S19] C：快速排序
来源：http://mobile.fehbvm.com/Article/details/ggwbpshoc.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fehbvm.com/Article/details/gxgrcwnjl.sHtML

[S20] C：二分查找
来源：http://www.m.share.hesvh.cn/Article/details/gjxsxygji.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.zdbjq.cn/Article/details/ggsnbkfsg.sHtML

[S21] C：字符类别判断
来源：http://wap.zdbjq.cn/Article/details/gqncrsalv.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fehbvm.com/Article/details/gzvdbqrow.sHtML

[S22] C：字符串转数字
来源：http://m.share.zdbjq.cn/Article/details/gwznxvins.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.zdbjq.cn/Article/details/gufpvkuww.sHtML

[S23] C：随机数
来源：http://www.m.share.zdbjq.cn/Article/details/ginwwoogn.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fehbvm.com/Article/details/gnqqkcqbs.sHtML

[S24] C：获取本地时间
来源：http://www.share.hesvh.cn/Article/details/ggqmgvnsc.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.hesvh.cn/Article/details/gbyeutmgm.sHtML

[S25] C：内存拷贝
来源：http://www.blog.zdbjq.cn/Article/details/giitscxfh.sHtML

memcpy(dst, src, n);
来源：http://read.share.fehbvm.com/Article/details/gjylcknib.sHtML

[S26] C：内存清零
来源：http://www.share.fehbvm.com/Article/details/gmvavanwz.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.fehbvm.com/Article/details/gwaqvqkmy.sHtML

[S27] C：定义常量
来源：http://www.blog.fehbvm.com/Article/details/gquopfxex.sHtML

const double PI = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/guxairnft.sHtML

[S28] C：静态变量
来源：http://3g.hesvh.cn/Article/details/gienuidtl.sHtML

static int counter = 0;
来源：http://3g.zdbjq.cn/Article/details/gmdnyqiav.sHtML

[S29] C：变参函数
来源：http://www.m.share.hesvh.cn/Article/details/gorpictqv.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.zdbjq.cn/Article/details/gmyekvqfp.sHtML

[S30] C：头文件保护
来源：http://read.share.zdbjq.cn/Article/details/ghqbclbss.sHtML

#ifndef X_H
来源：http://read.share.fehbvm.com/Article/details/gbkvkocds.sHtML

#define X_H
来源：http://baike.zdbjq.cn/Article/details/gjgqijrtd.sHtML

#endif
来源：http://blog.zdbjq.cn/Article/details/gtcckeeqq.sHtML

[S31] C++：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gxgigdsmi.sHtML

#include <iostream>
来源：http://wap.zdbjq.cn/Article/details/gzbyduird.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.zdbjq.cn/Article/details/gkewmzxdd.sHtML

[S32] C++：字符串
来源：http://blog.fehbvm.com/Article/details/gmwisjfvc.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.zdbjq.cn/Article/details/glcruyild.sHtML

[S33] C++：vector 增删
来源：http://read.share.hesvh.cn/Article/details/gixdoxgzl.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.zdbjq.cn/Article/details/grxblkdxv.sHtML

[S34] C++：遍历 vector
来源：http://blog.fehbvm.com/Article/details/gdzqbggdk.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.fehbvm.com/Article/details/gktqdexdv.sHtML

[S35] C++：map
来源：http://mobile.fehbvm.com/Article/details/gpszentcm.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gygdqcrxt.sHtML

[S36] C++：unordered_map
来源：http://www.blog.zdbjq.cn/Article/details/gvgjmherl.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gxzkpfofp.sHtML

[S37] C++：set
来源：http://wap.hesvh.cn/Article/details/glhheshkc.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.fehbvm.com/Article/details/gbtkwewft.sHtML

[S38] C++：排序
来源：http://m.share.zdbjq.cn/Article/details/ghznzoirm.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.fehbvm.com/Article/details/gzjlwbhhd.sHtML


<!-- 参考信息 -->