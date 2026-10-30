代发 wailian999

ANALYZE TABLE users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gsdmqdqzj.sHtML

[Q71] 查看建表语句
来源：http://read.share.fanxiaobao.xyz/Article/details/gheezkbav.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvagshxxm.sHtML

[Q72] 查看索引
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grntoxzwr.sHtML

SHOW INDEX FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gmtiwydaj.sHtML

[Q73] 查看表状态
来源：http://www.blog.fanxiaobao.xyz/Article/details/guscgycyn.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.fanxiaobao.xyz/Article/details/gwrxdjlsy.sHtML

[Q74] 强制使用索引
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcgmtllaz.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.fanxiaobao.xyz/Article/details/grtvpwwwq.sHtML

[Q75] 日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gplvquoth.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/grhfrfcfc.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.fanxiaobao.xyz/Article/details/gfzszcbtb.sHtML

[Q76] 按天统计
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvppclwes.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.fanxiaobao.xyz/Article/details/gvuxkucki.sHtML

[Q77] 时间加减
来源：http://m.share.fanxiaobao.xyz/Article/details/gswqnzzot.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.fanxiaobao.xyz/Article/details/gmsdurwqw.sHtML

[Q78] 当前时间
来源：http://wap.fanxiaobao.xyz/Article/details/gljqfsrku.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gelyxercw.sHtML

[Q79] 字符串拼接
来源：http://read.share.fanxiaobao.xyz/Article/details/grjgvzqge.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.fanxiaobao.xyz/Article/details/gmxtxghyx.sHtML

[Q80] 字符串截取
来源：http://read.share.fanxiaobao.xyz/Article/details/gjjzazvoj.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gtsptorzu.sHtML

[Q81] 字符串替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gnvxaiora.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbbhzyfzy.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbupfmyei.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gozvjseqv.sHtML

[Q83] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyhemdhhp.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghiilvnlf.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsivrcaxk.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gffnogwrh.sHtML

[Q85] 数值取整
来源：http://3g.fanxiaobao.xyz/Article/details/ggqlhlkuc.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.fanxiaobao.xyz/Article/details/geqbtgayw.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.fanxiaobao.xyz/Article/details/glmhddbkm.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.fanxiaobao.xyz/Article/details/gerccklzs.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gybzasdwh.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.fanxiaobao.xyz/Article/details/gxpvuxfsq.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwntjlgkq.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.fanxiaobao.xyz/Article/details/gconxhacs.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/glgujrqsv.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gopmdwqfo.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.fanxiaobao.xyz/Article/details/guevvpcer.sHtML

[Q90] 生成序号列
来源：http://blog.fanxiaobao.xyz/Article/details/gkyozwqke.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.fanxiaobao.xyz/Article/details/gmbynoprf.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/goujkrahs.sHtML

R. Bash 专题
来源：http://mobile.fanxiaobao.xyz/Article/details/gwcnporlg.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gtmjedbpl.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpsqlnwuf.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyacfbhgm.sHtML

set -euo pipefail
来源：http://wap.fanxiaobao.xyz/Article/details/glqjpidej.sHtML

[R02] 变量赋值与使用
来源：http://read.share.fanxiaobao.xyz/Article/details/gvqiedrby.sHtML

name="Tom"; echo "$name"
来源：http://mobile.fanxiaobao.xyz/Article/details/gppbvpnqp.sHtML

[R03] 只读变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gxmbxlcle.sHtML

readonly PI=3.14
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guyviwgfm.sHtML

[R04] 位置参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gtfpmfahh.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gojqtugun.sHtML

[R05] 参数默认值
来源：http://www.share.fanxiaobao.xyz/Article/details/gqarucvwf.sHtML

name="${1:-default}"
来源：http://baike.fanxiaobao.xyz/Article/details/gsmvlumbp.sHtML

[R06] 判断命令是否存在
来源：http://3g.fanxiaobao.xyz/Article/details/gvptyorfu.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqztxfsfc.sHtML

[R07] if 判断文件
来源：http://www.share.fanxiaobao.xyz/Article/details/ggguvhdkv.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gwtgvbkco.sHtML

[R08] 数值比较
来源：http://blog.fanxiaobao.xyz/Article/details/gqkrpxaco.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcmspexim.sHtML

[R09] 字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/gewqfzgvq.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/grdfcgpbn.sHtML

[R10] 正则匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/gtqzpqbpa.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gnxswowvj.sHtML

[R11] case 多分支
来源：http://baike.fanxiaobao.xyz/Article/details/gpfoxoozq.sHtML

case "$1" in
来源：http://blog.fanxiaobao.xyz/Article/details/gnnldntyl.sHtML

start) echo "启动" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gopkoonfl.sHtML

stop)  echo "停止" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gjbyydpvu.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gulvzhzju.sHtML

esac
来源：http://www.share.fanxiaobao.xyz/Article/details/gduqnsjmw.sHtML

[R12] for 遍历文件
来源：http://baike.fanxiaobao.xyz/Article/details/guqelfdws.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gorjmfssz.sHtML

[R13] for 计数循环
来源：http://3g.fanxiaobao.xyz/Article/details/grzxuidmc.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.fanxiaobao.xyz/Article/details/govcsajbf.sHtML

[R14] C 风格 for
来源：http://baike.fanxiaobao.xyz/Article/details/gxikwkdvz.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkvucunxh.sHtML

[R15] while 逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gzdtpgytl.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gqqhipwvx.sHtML

[R16] until 等待条件
来源：http://3g.fanxiaobao.xyz/Article/details/gbfbybswo.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gxedmjxya.sHtML

[R17] 数组定义与取值
来源：http://m.share.fanxiaobao.xyz/Article/details/gnsiobomh.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gbfzcszig.sHtML

[R18] 遍历数组
来源：http://m.share.fanxiaobao.xyz/Article/details/ggpaxuhee.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfuklgspv.sHtML

[R19] 数组长度
来源：http://baike.fanxiaobao.xyz/Article/details/gckiiwqzx.sHtML

echo "${#arr[@]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gcuhcarbp.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkjjkpwbd.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gnpoqbzia.sHtML

[R21] 字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/gmutsmldi.sHtML

echo "${#s}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnlxnsrin.sHtML

[R22] 截取子串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gajqjkegp.sHtML

echo "${s:0:5}"
来源：http://3g.fanxiaobao.xyz/Article/details/gvjcvtght.sHtML

[R23] 字符串替换
来源：http://baike.fanxiaobao.xyz/Article/details/gnwrqtwvr.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gedxhbtvk.sHtML

[R24] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwlbnktep.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gmocggkjf.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.fanxiaobao.xyz/Article/details/grolrdozi.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gjbuoleyl.sHtML

[R26] 命令替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gpyekbdxd.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxsukkzhe.sHtML

[R27] 算术展开
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjkerzhrc.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.fanxiaobao.xyz/Article/details/gvzzsfyee.sHtML

[R28] 浮点运算
来源：http://blog.fanxiaobao.xyz/Article/details/ggcvzzkqk.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.fanxiaobao.xyz/Article/details/gygmmenfz.sHtML

[R29] 定义函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdknbdpyh.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gqbukbeah.sHtML

[R30] 函数返回状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/gjdtuwcgt.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fanxiaobao.xyz/Article/details/gedinzcho.sHtML

[R31] 局部变量
来源：http://baike.fanxiaobao.xyz/Article/details/gxqupshxn.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gvucwltrs.sHtML

[R32] 参数个数校验
来源：http://mobile.fanxiaobao.xyz/Article/details/gnfcqcnoc.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwlojnxup.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fanxiaobao.xyz/Article/details/ghiwaffgw.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.fanxiaobao.xyz/Article/details/gyvwzkojs.sHtML

[R34] 退出时清理
来源：http://read.share.fanxiaobao.xyz/Article/details/gjmqpfqrn.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/gxwowyqgk.sHtML

[R35] 后台执行并等待
来源：http://wap.fanxiaobao.xyz/Article/details/gkzkkqdnu.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.fanxiaobao.xyz/Article/details/gcukqxvtn.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmndsufrw.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.fanxiaobao.xyz/Article/details/ggfdpyqwx.sHtML

[R37] 把输出赋给变量
来源：http://m.share.fanxiaobao.xyz/Article/details/getyusojf.sHtML

files=$(ls -1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gtwbptpym.sHtML

[R38] 管道串联
来源：http://m.share.fanxiaobao.xyz/Article/details/gbshhhsha.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fanxiaobao.xyz/Article/details/gzcmwwkkf.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.fanxiaobao.xyz/Article/details/giyrpdxtz.sHtML

cmd > out.log 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/gpbaabadg.sHtML

[R40] 追加写日志
来源：http://blog.fanxiaobao.xyz/Article/details/gyreejaae.sHtML

echo "log" >> out.log
来源：http://wap.fanxiaobao.xyz/Article/details/gbgpgqwqg.sHtML

[R41] 丢弃输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtnnhbdlq.sHtML

cmd >/dev/null 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/getvaducd.sHtML

[R42] 输入重定向
来源：http://wap.fanxiaobao.xyz/Article/details/gmxjflgmb.sHtML

wc -l < a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxhheighm.sHtML

[R43] 按名字查找文件
来源：http://blog.fanxiaobao.xyz/Article/details/gahryltan.sHtML

find . -name "*.log" -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/gyylyrhjm.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpubeoljl.sHtML

find . -mtime -7 -type f
来源：http://read.share.fanxiaobao.xyz/Article/details/gngvbxltq.sHtML

[R45] 批量删除
来源：http://baike.fanxiaobao.xyz/Article/details/gcbwlvpsy.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.fanxiaobao.xyz/Article/details/gewhfauoy.sHtML

[R46] 递归替换文件内容
来源：http://blog.fanxiaobao.xyz/Article/details/gvitfskoo.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fanxiaobao.xyz/Article/details/gvfzksivk.sHtML

[R47] sed 单行替换
来源：http://3g.fanxiaobao.xyz/Article/details/gswaobzna.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gqhtfvigz.sHtML

[R48] awk 取指定列
来源：http://www.share.fanxiaobao.xyz/Article/details/gprxqcfdj.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gclyheqly.sHtML

[R49] awk 带条件
来源：http://blog.fanxiaobao.xyz/Article/details/ghzkjdehg.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fanxiaobao.xyz/Article/details/gykutrjvc.sHtML

[R50] awk 求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gudzjhqqg.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gafbhnrjx.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqhsktsln.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fanxiaobao.xyz/Article/details/gnicoqupr.sHtML

[R52] 统计行数
来源：http://mobile.fanxiaobao.xyz/Article/details/gbflojaoz.sHtML

wc -l a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/grqfvhumq.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.fanxiaobao.xyz/Article/details/glphorkgk.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fanxiaobao.xyz/Article/details/gtzkedbdc.sHtML

[R54] 比较两个文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqthbsxry.sHtML

diff a.txt b.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/grlhyubqv.sHtML

[R55] 压缩与解压
来源：http://www.share.fanxiaobao.xyz/Article/details/gkciaussk.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fanxiaobao.xyz/Article/details/gtkpyjuol.sHtML

[R56] 远程拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/gizzeeuam.sHtML

scp file user@host:/path/
来源：http://wap.fanxiaobao.xyz/Article/details/gecqphspd.sHtML

[R57] 远程执行命令
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnzdpebdi.sHtML

ssh user@host 'uptime'
来源：http://mobile.fanxiaobao.xyz/Article/details/gsygnsrgq.sHtML

[R58] 下载文件
来源：http://blog.fanxiaobao.xyz/Article/details/gynatcefo.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.fanxiaobao.xyz/Article/details/grrkocajz.sHtML

[R59] 发 POST JSON
来源：http://baike.fanxiaobao.xyz/Article/details/gvkmsxjgi.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fanxiaobao.xyz/Article/details/goldcpoji.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gyombjwtc.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fanxiaobao.xyz/Article/details/gjbeyvuxw.sHtML

[R61] 磁盘占用
来源：http://blog.fanxiaobao.xyz/Article/details/gdilyjfbn.sHtML

df -h;  du -sh *
来源：http://baike.fanxiaobao.xyz/Article/details/gewhaeuud.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gtiavoieq.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fanxiaobao.xyz/Article/details/gmwsvnees.sHtML

[R63] 内存与进程
来源：http://blog.fanxiaobao.xyz/Article/details/gitfqyfzy.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.fanxiaobao.xyz/Article/details/gsobilioi.sHtML

[R64] 结束进程
来源：http://www.share.fanxiaobao.xyz/Article/details/gzprewhlj.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjyqtjyhj.sHtML

[R65] 查看端口占用
来源：http://blog.fanxiaobao.xyz/Article/details/gdsdpcpnb.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.fanxiaobao.xyz/Article/details/gmjfriove.sHtML

[R66] 定时任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghtyfzyjm.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdztnphfs.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmfqcmdym.sHtML

openssl rand -hex 16
来源：http://3g.fanxiaobao.xyz/Article/details/gfjxqlhsz.sHtML

[R68] 计算文件校验值
来源：http://mobile.fanxiaobao.xyz/Article/details/gdhanfuuk.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gvkxszfpa.sHtML

[R69] 生成随机密码
来源：http://wap.fanxiaobao.xyz/Article/details/goqblafrn.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fanxiaobao.xyz/Article/details/glyuzxhxz.sHtML

[R70] 时间戳与互转
来源：http://wap.fanxiaobao.xyz/Article/details/gkgbasghu.sHtML

date +%s;  date -d @1700000000
来源：http://blog.fanxiaobao.xyz/Article/details/gpgufgudc.sHtML

[R71] 日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwrwsuabl.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fanxiaobao.xyz/Article/details/gchednwta.sHtML

[R72] 等待端口就绪
来源：http://blog.fanxiaobao.xyz/Article/details/girzwmafk.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/gnfufenfn.sHtML

[R73] 分割大日志
来源：http://wap.fanxiaobao.xyz/Article/details/giudlgmkq.sHtML

split -l 1000 big.log part_
来源：http://m.share.fanxiaobao.xyz/Article/details/gxltghngw.sHtML

[R74] 批量重命名
来源：http://baike.fanxiaobao.xyz/Article/details/gjmrgqkpe.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gsupncdee.sHtML

[R75] 导出环境变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giseqpjwi.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.fanxiaobao.xyz/Article/details/gcniisumj.sHtML

[R76] 使用临时文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gnwcswnkw.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/gibkngmpl.sHtML

[R77] 读取用户输入
来源：http://blog.fanxiaobao.xyz/Article/details/gakbtgzua.sHtML

read -rp "请输入: " ans
来源：http://blog.fanxiaobao.xyz/Article/details/ggmydcbap.sHtML

[R78] 交互式菜单
来源：http://blog.fanxiaobao.xyz/Article/details/gmhriyoru.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fanxiaobao.xyz/Article/details/gypmtzlab.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guzaigjwv.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gmzxvarfj.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fanxiaobao.xyz/Article/details/gjdgtfjdc.sHtML

time ./run.sh
来源：http://wap.fanxiaobao.xyz/Article/details/gfyoxvxnp.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gdidrcidy.sHtML

S. C / C++ 专题
来源：http://wap.fanxiaobao.xyz/Article/details/gshscffhf.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/grqlfgdjn.sHtML

[S01] C：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/genpbnmhf.sHtML

#include <stdio.h>
来源：http://3g.fanxiaobao.xyz/Article/details/grxecnsgo.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.fanxiaobao.xyz/Article/details/gaziipozw.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gnyidmddz.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fanxiaobao.xyz/Article/details/gaxbfhjef.sHtML

[S03] C：读入整数
来源：http://3g.fanxiaobao.xyz/Article/details/gwhkerswy.sHtML

int x; scanf("%d", &x);
来源：http://3g.fanxiaobao.xyz/Article/details/gqlbigdcc.sHtML

[S04] C：字符串复制
来源：http://m.share.fanxiaobao.xyz/Article/details/gusxscgae.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.fanxiaobao.xyz/Article/details/gpfhwtnxj.sHtML

[S05] C：字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gtgpdxzrb.sHtML

strlen(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glnpzjcha.sHtML

[S06] C：字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/gncizvsrx.sHtML

strcmp(a, b) == 0
来源：http://m.share.fanxiaobao.xyz/Article/details/gvzkqcwic.sHtML

[S07] C：数组遍历求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gaoqbwczk.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.fanxiaobao.xyz/Article/details/gndadervi.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fanxiaobao.xyz/Article/details/gzsldtrck.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.fanxiaobao.xyz/Article/details/grdhhglja.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.fanxiaobao.xyz/Article/details/gtpvzjvaf.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.fanxiaobao.xyz/Article/details/gzgosiipj.sHtML

[S10] C：指针与解引用
来源：http://www.blog.fanxiaobao.xyz/Article/details/goqiewibq.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fanxiaobao.xyz/Article/details/gjdfvcvsl.sHtML

[S11] C：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/ghmkwmgfa.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.fanxiaobao.xyz/Article/details/gtlhqfzzc.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.fanxiaobao.xyz/Article/details/ggbovaaou.sHtML

fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gnxgzprmd.sHtML

[S12] C：写文件
来源：http://blog.fanxiaobao.xyz/Article/details/gcqyvagps.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/gbaibpasj.sHtML

[S13] C：宏定义
来源：http://baike.fanxiaobao.xyz/Article/details/gahelqjrb.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.fanxiaobao.xyz/Article/details/gklemminx.sHtML

[S14] C：枚举
来源：http://baike.fanxiaobao.xyz/Article/details/gxsbakxgt.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdwjzgime.sHtML

[S15] C：类型转换
来源：http://wap.fanxiaobao.xyz/Article/details/gjbhthjun.sHtML

(double) a / b
来源：http://wap.fanxiaobao.xyz/Article/details/gbetmfqle.sHtML

[S16] C：位操作置位
来源：http://read.share.fanxiaobao.xyz/Article/details/guduzsgqo.sHtML

x |= (1 << 3);
来源：http://3g.fanxiaobao.xyz/Article/details/ggwpuuryq.sHtML

[S17] C：安全拼接字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gpttigmjy.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.fanxiaobao.xyz/Article/details/gmfalbevz.sHtML

[S18] C：命令行参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gzyharnnw.sHtML

int main(int argc, char **argv)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdwkjynim.sHtML

[S19] C：快速排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gcevvknut.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggzmqhxic.sHtML

[S20] C：二分查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghuyyijxn.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/gohwawkpr.sHtML

[S21] C：字符类别判断
来源：http://m.share.fanxiaobao.xyz/Article/details/ghirqgome.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcxcfyaxu.sHtML

[S22] C：字符串转数字
来源：http://m.share.fanxiaobao.xyz/Article/details/gdjzwjgbv.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fanxiaobao.xyz/Article/details/gltodzqst.sHtML

[S23] C：随机数
来源：http://3g.fanxiaobao.xyz/Article/details/gmlbggebl.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwhkykhwt.sHtML

[S24] C：获取本地时间
来源：http://3g.fanxiaobao.xyz/Article/details/gnidzzxmj.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fanxiaobao.xyz/Article/details/gunxpzmte.sHtML

[S25] C：内存拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/glmwvuvyi.sHtML

memcpy(dst, src, n);
来源：http://wap.fanxiaobao.xyz/Article/details/gzrwptiwg.sHtML

[S26] C：内存清零
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbgwnyxxf.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdfmazjdn.sHtML

[S27] C：定义常量
来源：http://blog.fanxiaobao.xyz/Article/details/gzjfogurd.sHtML

const double PI = 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gihtcdwje.sHtML

[S28] C：静态变量
来源：http://blog.fanxiaobao.xyz/Article/details/gvacugtgh.sHtML

static int counter = 0;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpkdxzfxq.sHtML

[S29] C：变参函数
来源：http://blog.fanxiaobao.xyz/Article/details/gjizjpykk.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fanxiaobao.xyz/Article/details/gyznisadg.sHtML

[S30] C：头文件保护
来源：http://wap.fanxiaobao.xyz/Article/details/gdohpisxw.sHtML

#ifndef X_H
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvdavyzrg.sHtML

#define X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gijfzytwh.sHtML

#endif
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmdchfwed.sHtML

[S31] C++：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gwxvofvom.sHtML

#include <iostream>
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkbkbqohg.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzlnwkolw.sHtML

[S32] C++：字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsvuuiziu.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.fanxiaobao.xyz/Article/details/gkfhflpzw.sHtML

[S33] C++：vector 增删
来源：http://3g.fanxiaobao.xyz/Article/details/gbmeudozh.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gqyxkstfb.sHtML

[S34] C++：遍历 vector
来源：http://m.share.fanxiaobao.xyz/Article/details/gduwakewm.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gpiaabuto.sHtML

[S35] C++：map
来源：http://baike.fanxiaobao.xyz/Article/details/ggphhxatj.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gpeftelin.sHtML

[S36] C++：unordered_map
来源：http://wap.fanxiaobao.xyz/Article/details/gjlznwrwt.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gujzpwqob.sHtML

[S37] C++：set
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcrqzccuw.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.fanxiaobao.xyz/Article/details/goaxedzuz.sHtML

[S38] C++：排序
来源：http://blog.fanxiaobao.xyz/Article/details/gxgvkjdhg.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.fanxiaobao.xyz/Article/details/gtlpiyhdo.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gxzggzczz.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fanxiaobao.xyz/Article/details/gepusyxjh.sHtML

[S40] C++：查找元素
来源：http://mobile.fanxiaobao.xyz/Article/details/ghrtnkszj.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glaqttmpo.sHtML


<!-- 参考信息 -->