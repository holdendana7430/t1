代发 wailian999

ROLLBACK TO sp1;
来源：http://mobile.fanxiaobao.xyz/Article/details/geqvoyhba.sHtML

[Q69] 查看执行计划
来源：http://www.blog.fanxiaobao.xyz/Article/details/gslkahkgf.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdayonhzk.sHtML

[Q70] 更新统计信息
来源：http://m.share.fanxiaobao.xyz/Article/details/gqbzmnkia.sHtML

ANALYZE TABLE users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gtxprmnfm.sHtML

[Q71] 查看建表语句
来源：http://wap.fanxiaobao.xyz/Article/details/gnbcdfggu.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.fanxiaobao.xyz/Article/details/gqifdsppm.sHtML

[Q72] 查看索引
来源：http://mobile.fanxiaobao.xyz/Article/details/ganidtydi.sHtML

SHOW INDEX FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gwrmtuwhp.sHtML

[Q73] 查看表状态
来源：http://wap.fanxiaobao.xyz/Article/details/gfwisndgd.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.fanxiaobao.xyz/Article/details/gmrlkxypt.sHtML

[Q74] 强制使用索引
来源：http://www.share.fanxiaobao.xyz/Article/details/glarasobn.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnhinnwnp.sHtML

[Q75] 日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtwjkkjfu.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbmjuhwgf.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.fanxiaobao.xyz/Article/details/gbrkmmwkn.sHtML

[Q76] 按天统计
来源：http://3g.fanxiaobao.xyz/Article/details/gdrhffime.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbyhhhjja.sHtML

[Q77] 时间加减
来源：http://baike.fanxiaobao.xyz/Article/details/gkjvgevxz.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.fanxiaobao.xyz/Article/details/grncsutmg.sHtML

[Q78] 当前时间
来源：http://m.share.fanxiaobao.xyz/Article/details/gwkesiods.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.fanxiaobao.xyz/Article/details/gasjjgsxb.sHtML

[Q79] 字符串拼接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpkwbsaaz.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gibhlbjrp.sHtML

[Q80] 字符串截取
来源：http://www.blog.fanxiaobao.xyz/Article/details/getorgtwl.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gpiicxyxl.sHtML

[Q81] 字符串替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gofkhcbgk.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjladagjy.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gnvtrffjw.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gfubgwkcr.sHtML

[Q83] 大小写转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gxfaytkxh.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/glibnlqir.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbdsqnqqz.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/goimgppfl.sHtML

[Q85] 数值取整
来源：http://baike.fanxiaobao.xyz/Article/details/gbenytavq.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.fanxiaobao.xyz/Article/details/gqlvjuxbg.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.fanxiaobao.xyz/Article/details/gumbzbcxp.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyktndgrc.sHtML

[Q87] JSON 字段做条件
来源：http://blog.fanxiaobao.xyz/Article/details/gbdbkhylk.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjegzqvsk.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.fanxiaobao.xyz/Article/details/gkrvpatgz.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.fanxiaobao.xyz/Article/details/gbidwwtye.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/ggjsvxwvb.sHtML

[Q89] 判断表是否存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gcnwqnkbb.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.fanxiaobao.xyz/Article/details/goxasaqug.sHtML

[Q90] 生成序号列
来源：http://wap.fanxiaobao.xyz/Article/details/gpbtjrnnp.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gugazwnyz.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gzzknsbmk.sHtML

R. Bash 专题
来源：http://www.share.fanxiaobao.xyz/Article/details/gisykibio.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/glstqpgnz.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdckpdrdp.sHtML

#!/usr/bin/env bash
来源：http://www.blog.fanxiaobao.xyz/Article/details/goplxihza.sHtML

set -euo pipefail
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdtvxkydj.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gffwskxny.sHtML

name="Tom"; echo "$name"
来源：http://m.share.fanxiaobao.xyz/Article/details/gbennzyro.sHtML

[R03] 只读变量
来源：http://wap.fanxiaobao.xyz/Article/details/gidhlugsc.sHtML

readonly PI=3.14
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpfkypjnz.sHtML

[R04] 位置参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnshrevtg.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.fanxiaobao.xyz/Article/details/gjicfjfqs.sHtML

[R05] 参数默认值
来源：http://wap.fanxiaobao.xyz/Article/details/guvcjvpzd.sHtML

name="${1:-default}"
来源：http://3g.fanxiaobao.xyz/Article/details/gfhpijchj.sHtML

[R06] 判断命令是否存在
来源：http://blog.fanxiaobao.xyz/Article/details/gxozwidxx.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gakixloux.sHtML

[R07] if 判断文件
来源：http://blog.fanxiaobao.xyz/Article/details/guivzlncz.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gvivwvpvr.sHtML

[R08] 数值比较
来源：http://wap.fanxiaobao.xyz/Article/details/gpnzwnnis.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyvudqgsb.sHtML

[R09] 字符串比较
来源：http://wap.fanxiaobao.xyz/Article/details/gkggvqesr.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtdwkgimt.sHtML

[R10] 正则匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/gxqpzkwzq.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzjhqrnxa.sHtML

[R11] case 多分支
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmhfcmglx.sHtML

case "$1" in
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gprdzosmh.sHtML

start) echo "启动" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gircqsobr.sHtML

stop)  echo "停止" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/gssfntdmu.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/graqrptwi.sHtML

esac
来源：http://m.share.fanxiaobao.xyz/Article/details/gjxwwwhlk.sHtML

[R12] for 遍历文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdsyprayu.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/giwzzfxdq.sHtML

[R13] for 计数循环
来源：http://baike.fanxiaobao.xyz/Article/details/gzldxfyzt.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/glbzpazdr.sHtML

[R14] C 风格 for
来源：http://m.share.fanxiaobao.xyz/Article/details/gluysztrr.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gbvsqvzzc.sHtML

[R15] while 逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/goyxlognw.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gjsshreuh.sHtML

[R16] until 等待条件
来源：http://m.share.fanxiaobao.xyz/Article/details/grdfwoieh.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gmdmxxqds.sHtML

[R17] 数组定义与取值
来源：http://read.share.fanxiaobao.xyz/Article/details/gmaupxszk.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpgjmszvb.sHtML

[R18] 遍历数组
来源：http://m.share.fanxiaobao.xyz/Article/details/gvnrslwkp.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.fanxiaobao.xyz/Article/details/glvcsijfn.sHtML

[R19] 数组长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvhorliwd.sHtML

echo "${#arr[@]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gdmyvkozm.sHtML

[R20] 关联数组（字典）
来源：http://read.share.fanxiaobao.xyz/Article/details/gszhtggvh.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gluloyjgw.sHtML

[R21] 字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnuinteqk.sHtML

echo "${#s}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gzjoymxnx.sHtML

[R22] 截取子串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcqyvxspb.sHtML

echo "${s:0:5}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gmgspqzny.sHtML

[R23] 字符串替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gctarpbri.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gsoqzaraq.sHtML

[R24] 大小写转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gbccrgtak.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqilvfgug.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.fanxiaobao.xyz/Article/details/gbhdivwvu.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gqdticarg.sHtML

[R26] 命令替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gqzkbqpiv.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.fanxiaobao.xyz/Article/details/gbwmklmqh.sHtML

[R27] 算术展开
来源：http://wap.fanxiaobao.xyz/Article/details/glpqkopqw.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjaisparv.sHtML

[R28] 浮点运算
来源：http://mobile.fanxiaobao.xyz/Article/details/gkvdceeos.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fanxiaobao.xyz/Article/details/grnfqvdeq.sHtML

[R29] 定义函数
来源：http://mobile.fanxiaobao.xyz/Article/details/geytxdmdq.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.fanxiaobao.xyz/Article/details/gwsgzfmjx.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvaevsbmc.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdwtvpdxt.sHtML

[R31] 局部变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gadhzlpyt.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gyamwgayw.sHtML

[R32] 参数个数校验
来源：http://www.blog.fanxiaobao.xyz/Article/details/gexhdtvxn.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gcpdzkkhn.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fanxiaobao.xyz/Article/details/gqbrfiqiw.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.fanxiaobao.xyz/Article/details/gthhztbsr.sHtML

[R34] 退出时清理
来源：http://blog.fanxiaobao.xyz/Article/details/gbfnmwomn.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/grsdmhbmx.sHtML

[R35] 后台执行并等待
来源：http://read.share.fanxiaobao.xyz/Article/details/gtotmbluf.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbtzojdik.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fanxiaobao.xyz/Article/details/ghxqlhygc.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.fanxiaobao.xyz/Article/details/gtufnbril.sHtML

[R37] 把输出赋给变量
来源：http://wap.fanxiaobao.xyz/Article/details/gbgrpjxru.sHtML

files=$(ls -1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbklameqs.sHtML

[R38] 管道串联
来源：http://wap.fanxiaobao.xyz/Article/details/gohtazhqf.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fanxiaobao.xyz/Article/details/gbismfljn.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.fanxiaobao.xyz/Article/details/glnxywrln.sHtML

cmd > out.log 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gcycofgpy.sHtML

[R40] 追加写日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxuhecxoz.sHtML

echo "log" >> out.log
来源：http://blog.fanxiaobao.xyz/Article/details/gadjizbas.sHtML

[R41] 丢弃输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gsppaovpj.sHtML

cmd >/dev/null 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gjqxnrfus.sHtML

[R42] 输入重定向
来源：http://read.share.fanxiaobao.xyz/Article/details/gaifhckzz.sHtML

wc -l < a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gzifyiudm.sHtML

[R43] 按名字查找文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggqccdqll.sHtML

find . -name "*.log" -type f
来源：http://blog.fanxiaobao.xyz/Article/details/gxlkjlltr.sHtML

[R44] 按修改时间查找
来源：http://www.share.fanxiaobao.xyz/Article/details/gnevmyqsj.sHtML

find . -mtime -7 -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/gpnskymfk.sHtML

[R45] 批量删除
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjlxqakrz.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fanxiaobao.xyz/Article/details/gxuvegjqe.sHtML

[R46] 递归替换文件内容
来源：http://baike.fanxiaobao.xyz/Article/details/goqexkczr.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fanxiaobao.xyz/Article/details/goskwxavy.sHtML

[R47] sed 单行替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gpygoqnnu.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvlrxiart.sHtML

[R48] awk 取指定列
来源：http://read.share.fanxiaobao.xyz/Article/details/giuezucol.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghnnxekfo.sHtML

[R49] awk 带条件
来源：http://wap.fanxiaobao.xyz/Article/details/glyxudxtz.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.fanxiaobao.xyz/Article/details/gpfvapgyi.sHtML

[R50] awk 求和
来源：http://mobile.fanxiaobao.xyz/Article/details/geiqnugom.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/ggtkgnoyo.sHtML

[R51] 排序去重取前几
来源：http://blog.fanxiaobao.xyz/Article/details/gqanuassd.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.fanxiaobao.xyz/Article/details/gdbsveoee.sHtML

[R52] 统计行数
来源：http://blog.fanxiaobao.xyz/Article/details/grjkjclna.sHtML

wc -l a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gwtdopawd.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fanxiaobao.xyz/Article/details/gbxtzejjr.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.fanxiaobao.xyz/Article/details/gibbsjyuw.sHtML

[R54] 比较两个文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkofvweqi.sHtML

diff a.txt b.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/glqvfctrk.sHtML

[R55] 压缩与解压
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyyohxbiy.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.fanxiaobao.xyz/Article/details/goppxuapv.sHtML

[R56] 远程拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gsfovdyba.sHtML

scp file user@host:/path/
来源：http://baike.fanxiaobao.xyz/Article/details/gmdjrkfsx.sHtML

[R57] 远程执行命令
来源：http://3g.fanxiaobao.xyz/Article/details/govfpjfbl.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvwnemjmy.sHtML

[R58] 下载文件
来源：http://mobile.fanxiaobao.xyz/Article/details/geciltbpo.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fanxiaobao.xyz/Article/details/gjxqzvtgc.sHtML

[R59] 发 POST JSON
来源：http://blog.fanxiaobao.xyz/Article/details/gtdkfbkls.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.fanxiaobao.xyz/Article/details/gfzobuybw.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.fanxiaobao.xyz/Article/details/gfvnrihkz.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.fanxiaobao.xyz/Article/details/gnddcxdtl.sHtML

[R61] 磁盘占用
来源：http://www.share.fanxiaobao.xyz/Article/details/gfupebknt.sHtML

df -h;  du -sh *
来源：http://www.share.fanxiaobao.xyz/Article/details/gakpyfyeb.sHtML

[R62] 找最占空间的文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gnjvfdouf.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fanxiaobao.xyz/Article/details/grwpalaxe.sHtML

[R63] 内存与进程
来源：http://wap.fanxiaobao.xyz/Article/details/gdkjlaoxr.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.fanxiaobao.xyz/Article/details/gnzlqmhdh.sHtML

[R64] 结束进程
来源：http://3g.fanxiaobao.xyz/Article/details/gwwigetto.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.fanxiaobao.xyz/Article/details/ghjkqfxez.sHtML

[R65] 查看端口占用
来源：http://read.share.fanxiaobao.xyz/Article/details/gjztezkwb.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.fanxiaobao.xyz/Article/details/gujxsrxny.sHtML

[R66] 定时任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbakleqps.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqrcomlrk.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fanxiaobao.xyz/Article/details/gcghitmqm.sHtML

openssl rand -hex 16
来源：http://3g.fanxiaobao.xyz/Article/details/gcrnpoqew.sHtML

[R68] 计算文件校验值
来源：http://wap.fanxiaobao.xyz/Article/details/glmttjhlk.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gymuhzxmm.sHtML

[R69] 生成随机密码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gywoumylh.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fanxiaobao.xyz/Article/details/gjcnlydiu.sHtML

[R70] 时间戳与互转
来源：http://baike.fanxiaobao.xyz/Article/details/gzbxibgji.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghdlenvxl.sHtML

[R71] 日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gnfqgcaem.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyulexrci.sHtML

[R72] 等待端口就绪
来源：http://m.share.fanxiaobao.xyz/Article/details/ggtzmsgow.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvyhmxeqx.sHtML

[R73] 分割大日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gebryxwtz.sHtML

split -l 1000 big.log part_
来源：http://mobile.fanxiaobao.xyz/Article/details/gexppiwdw.sHtML

[R74] 批量重命名
来源：http://baike.fanxiaobao.xyz/Article/details/gecjfnpjq.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gpqdsmlfx.sHtML

[R75] 导出环境变量
来源：http://wap.fanxiaobao.xyz/Article/details/ghzqioagw.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.fanxiaobao.xyz/Article/details/gxpdslfri.sHtML

[R76] 使用临时文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/guvkbgjsv.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/gcqjphxhd.sHtML

[R77] 读取用户输入
来源：http://3g.fanxiaobao.xyz/Article/details/gqexxvsmb.sHtML

read -rp "请输入: " ans
来源：http://blog.fanxiaobao.xyz/Article/details/gjjoymftj.sHtML

[R78] 交互式菜单
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grepnxexs.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gchsmeitt.sHtML

[R79] 解析命令行选项
来源：http://3g.fanxiaobao.xyz/Article/details/gzbmvzlfx.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gcompyvoh.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbewldtav.sHtML

time ./run.sh
来源：http://www.share.fanxiaobao.xyz/Article/details/gqxbmcurp.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/geivymefy.sHtML

S. C / C++ 专题
来源：http://baike.fanxiaobao.xyz/Article/details/gfcosjoij.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goawkviap.sHtML

[S01] C：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghdfcvnbn.sHtML

#include <stdio.h>
来源：http://m.share.fanxiaobao.xyz/Article/details/gbrxcybeo.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.fanxiaobao.xyz/Article/details/gnykgmmqr.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gemttveue.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.fanxiaobao.xyz/Article/details/gfdhtiodh.sHtML

[S03] C：读入整数
来源：http://baike.fanxiaobao.xyz/Article/details/guxlsevom.sHtML

int x; scanf("%d", &x);
来源：http://3g.fanxiaobao.xyz/Article/details/gyakwslxk.sHtML

[S04] C：字符串复制
来源：http://blog.fanxiaobao.xyz/Article/details/gjeyteqft.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fanxiaobao.xyz/Article/details/gvqnusqxp.sHtML

[S05] C：字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gtcjyqfwg.sHtML

strlen(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gcpvudnrd.sHtML

[S06] C：字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gjbllyczg.sHtML

strcmp(a, b) == 0
来源：http://mobile.fanxiaobao.xyz/Article/details/gliejrdoq.sHtML

[S07] C：数组遍历求和
来源：http://blog.fanxiaobao.xyz/Article/details/gjudikqjc.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fanxiaobao.xyz/Article/details/gvxubdasz.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fanxiaobao.xyz/Article/details/grfkfyxki.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.fanxiaobao.xyz/Article/details/gmxzfljjp.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.fanxiaobao.xyz/Article/details/gpklnosfe.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmqdazfue.sHtML

[S10] C：指针与解引用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtsowptms.sHtML

int *p = &a;  *p = 5;
来源：http://3g.fanxiaobao.xyz/Article/details/gbglmlals.sHtML

[S11] C：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gazczpkop.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.fanxiaobao.xyz/Article/details/gmoobtqob.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gofpyxapx.sHtML

fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/gxofnctht.sHtML

[S12] C：写文件
来源：http://mobile.fanxiaobao.xyz/Article/details/giictejge.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/gioqnmdex.sHtML

[S13] C：宏定义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdqtyfbde.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghpkgwnsv.sHtML

[S14] C：枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/gljmdcygv.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.fanxiaobao.xyz/Article/details/gzsunrscp.sHtML

[S15] C：类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnmelohbu.sHtML

(double) a / b
来源：http://baike.fanxiaobao.xyz/Article/details/gsdbnkhfc.sHtML

[S16] C：位操作置位
来源：http://mobile.fanxiaobao.xyz/Article/details/ghohfvefs.sHtML

x |= (1 << 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gwhqytfyk.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtszxevgi.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggounepzf.sHtML

[S18] C：命令行参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbsgcvawy.sHtML

int main(int argc, char **argv)
来源：http://wap.fanxiaobao.xyz/Article/details/gxgfdgquh.sHtML

[S19] C：快速排序
来源：http://baike.fanxiaobao.xyz/Article/details/gqzngmxwu.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/gpxtbhnmg.sHtML

[S20] C：二分查找
来源：http://www.share.fanxiaobao.xyz/Article/details/gqftzkmqb.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/grshyrfcc.sHtML

[S21] C：字符类别判断
来源：http://read.share.fanxiaobao.xyz/Article/details/gnvizovxl.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fanxiaobao.xyz/Article/details/ghkshilmu.sHtML

[S22] C：字符串转数字
来源：http://3g.fanxiaobao.xyz/Article/details/ggjaiwpol.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fanxiaobao.xyz/Article/details/gaxaggvnz.sHtML

[S23] C：随机数
来源：http://www.share.fanxiaobao.xyz/Article/details/ghavbphra.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fanxiaobao.xyz/Article/details/gbgkgepxc.sHtML

[S24] C：获取本地时间
来源：http://baike.fanxiaobao.xyz/Article/details/gazusnwsg.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fanxiaobao.xyz/Article/details/gucnbkjtk.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtahrmqoa.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqurfnlwn.sHtML

[S26] C：内存清零
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzhkgmybc.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkgwcybcp.sHtML

[S27] C：定义常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gnzsjizni.sHtML

const double PI = 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnhuvnmjs.sHtML

[S28] C：静态变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gzudimczr.sHtML

static int counter = 0;
来源：http://www.share.fanxiaobao.xyz/Article/details/gxtjxiwvu.sHtML

[S29] C：变参函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gbpxtzexu.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fanxiaobao.xyz/Article/details/ghtxpnoep.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gduzatozw.sHtML

#ifndef X_H
来源：http://m.share.fanxiaobao.xyz/Article/details/gsrkeigdj.sHtML

#define X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/gtbldschf.sHtML

#endif
来源：http://read.share.fanxiaobao.xyz/Article/details/gcorjucvm.sHtML

[S31] C++：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gwrhbkaqy.sHtML

#include <iostream>
来源：http://blog.fanxiaobao.xyz/Article/details/gwugyrzin.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqihyddgc.sHtML

[S32] C++：字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gndxzeyac.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.fanxiaobao.xyz/Article/details/ggohlohem.sHtML

[S33] C++：vector 增删
来源：http://m.share.fanxiaobao.xyz/Article/details/gqnrmwljs.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gjrcvssvj.sHtML

[S34] C++：遍历 vector
来源：http://m.share.fanxiaobao.xyz/Article/details/gvlpnraoh.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.fanxiaobao.xyz/Article/details/gdojgxwsj.sHtML

[S35] C++：map
来源：http://baike.fanxiaobao.xyz/Article/details/ggvpjdkfb.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/goygeaskl.sHtML

[S36] C++：unordered_map
来源：http://wap.fanxiaobao.xyz/Article/details/gpwroxmuv.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/glykylsnq.sHtML

[S37] C++：set
来源：http://wap.fanxiaobao.xyz/Article/details/gvjqcmzam.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glpzzhsiw.sHtML

[S38] C++：排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gqxbnsqlm.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.fanxiaobao.xyz/Article/details/gvtwtsita.sHtML


<!-- 参考信息 -->