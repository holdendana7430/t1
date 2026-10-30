代发 wailian999

SHOW INDEX FROM users;
来源：http://www.share.fehbvm.com/Article/details/gwzfurcqx.sHtML

[Q73] 查看表状态
来源：http://m.share.zdbjq.cn/Article/details/grylnhafh.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.fehbvm.com/Article/details/gliffnlgr.sHtML

[Q74] 强制使用索引
来源：http://mobile.hesvh.cn/Article/details/gmafmpntt.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.fehbvm.com/Article/details/gsqogbraj.sHtML

[Q75] 日期格式化
来源：http://www.share.hesvh.cn/Article/details/gmuvsjpcg.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gllexdtrq.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.zdbjq.cn/Article/details/gvvcbiewv.sHtML

[Q76] 按天统计
来源：http://mobile.zdbjq.cn/Article/details/glashoeot.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.zdbjq.cn/Article/details/gkgdljytj.sHtML

[Q77] 时间加减
来源：http://blog.zdbjq.cn/Article/details/gnhavjqnv.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.zdbjq.cn/Article/details/gfddvvikj.sHtML

[Q78] 当前时间
来源：http://www.m.share.fehbvm.com/Article/details/gyvoxoxga.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.hesvh.cn/Article/details/gwmjuryco.sHtML

[Q79] 字符串拼接
来源：http://www.share.zdbjq.cn/Article/details/glofvcksh.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.hesvh.cn/Article/details/gigynxwtf.sHtML

[Q80] 字符串截取
来源：http://m.share.zdbjq.cn/Article/details/gmxnhwznl.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.hesvh.cn/Article/details/gwfktqqei.sHtML

[Q81] 字符串替换
来源：http://www.share.zdbjq.cn/Article/details/gxhpzmyza.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.hesvh.cn/Article/details/gpwivfuek.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.zdbjq.cn/Article/details/gwahgdiwg.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gxdortpjm.sHtML

[Q83] 大小写转换
来源：http://m.share.fehbvm.com/Article/details/gzcdxzbta.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.hesvh.cn/Article/details/gtwflnwtf.sHtML

[Q84] 去除首尾空格
来源：http://3g.fehbvm.com/Article/details/gagwecxkh.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/ggzgbgpjs.sHtML

[Q85] 数值取整
来源：http://baike.zdbjq.cn/Article/details/gifvysvdl.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.zdbjq.cn/Article/details/grexekiaj.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.hesvh.cn/Article/details/ggkbbxssk.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.fehbvm.com/Article/details/gmuhsvvwj.sHtML

[Q87] JSON 字段做条件
来源：http://wap.zdbjq.cn/Article/details/ghnbkfegh.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.hesvh.cn/Article/details/gloaotxnh.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.hesvh.cn/Article/details/gowoxcryb.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.zdbjq.cn/Article/details/gsquojnkn.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gtqbmjhbd.sHtML

[Q89] 判断表是否存在
来源：http://www.share.hesvh.cn/Article/details/gtppqbiue.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.hesvh.cn/Article/details/gpawjyxdl.sHtML

[Q90] 生成序号列
来源：http://www.blog.hesvh.cn/Article/details/gmerxwsoh.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.hesvh.cn/Article/details/gzzloxnpm.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/ghputpvnz.sHtML

R. Bash 专题
来源：http://wap.fehbvm.com/Article/details/gjdyltgvm.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gsoldntxl.sHtML

[R01] shebang 与严格模式
来源：http://mobile.zdbjq.cn/Article/details/guewmceuv.sHtML

#!/usr/bin/env bash
来源：http://mobile.hesvh.cn/Article/details/gsynafmfy.sHtML

set -euo pipefail
来源：http://baike.fehbvm.com/Article/details/gahyajpbs.sHtML

[R02] 变量赋值与使用
来源：http://blog.zdbjq.cn/Article/details/gplwzeavy.sHtML

name="Tom"; echo "$name"
来源：http://mobile.fehbvm.com/Article/details/gkgqelspi.sHtML

[R03] 只读变量
来源：http://m.share.fehbvm.com/Article/details/gsartjgtg.sHtML

readonly PI=3.14
来源：http://www.blog.fehbvm.com/Article/details/giuheshns.sHtML

[R04] 位置参数
来源：http://blog.fehbvm.com/Article/details/gemnfaiya.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.hesvh.cn/Article/details/gamvtoynh.sHtML

[R05] 参数默认值
来源：http://wap.hesvh.cn/Article/details/gjbvqrawj.sHtML

name="${1:-default}"
来源：http://read.share.fehbvm.com/Article/details/graexjcpe.sHtML

[R06] 判断命令是否存在
来源：http://3g.fehbvm.com/Article/details/gwqkkhysp.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.zdbjq.cn/Article/details/gwlxkaxls.sHtML

[R07] if 判断文件
来源：http://www.blog.fehbvm.com/Article/details/gqkbdxnsw.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.hesvh.cn/Article/details/ggxwznoly.sHtML

[R08] 数值比较
来源：http://www.m.share.zdbjq.cn/Article/details/gtylabizf.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.hesvh.cn/Article/details/gngnsjapb.sHtML

[R09] 字符串比较
来源：http://3g.zdbjq.cn/Article/details/ghengzvcs.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.hesvh.cn/Article/details/gtdvcqyll.sHtML

[R10] 正则匹配
来源：http://wap.fehbvm.com/Article/details/gearpgfvb.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.zdbjq.cn/Article/details/gzmgpopvm.sHtML

[R11] case 多分支
来源：http://www.share.fehbvm.com/Article/details/gquaoluqc.sHtML

case "$1" in
来源：http://m.share.zdbjq.cn/Article/details/gnsbszkte.sHtML

start) echo "启动" ;;
来源：http://wap.hesvh.cn/Article/details/gxbxalzjn.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.fehbvm.com/Article/details/gbmmemsgm.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.zdbjq.cn/Article/details/gbyzfswnu.sHtML

esac
来源：http://www.share.hesvh.cn/Article/details/gcnxmtrug.sHtML

[R12] for 遍历文件
来源：http://blog.fehbvm.com/Article/details/gsgfnvapt.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.hesvh.cn/Article/details/gzzlljadx.sHtML

[R13] for 计数循环
来源：http://www.m.share.zdbjq.cn/Article/details/gjyubacsi.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.zdbjq.cn/Article/details/gznfawney.sHtML

[R14] C 风格 for
来源：http://wap.hesvh.cn/Article/details/gepquhvwe.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.fehbvm.com/Article/details/glsezkcyr.sHtML

[R15] while 逐行读文件
来源：http://baike.fehbvm.com/Article/details/gnxtfugso.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.hesvh.cn/Article/details/gdhvezldg.sHtML

[R16] until 等待条件
来源：http://m.share.fehbvm.com/Article/details/gerqzdpjo.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.fehbvm.com/Article/details/gjrkrcqnj.sHtML

[R17] 数组定义与取值
来源：http://wap.fehbvm.com/Article/details/gchiwcrsh.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.zdbjq.cn/Article/details/glhuxcdnr.sHtML

[R18] 遍历数组
来源：http://m.share.hesvh.cn/Article/details/gpsjsvook.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.hesvh.cn/Article/details/gqtirqoko.sHtML

[R19] 数组长度
来源：http://3g.zdbjq.cn/Article/details/gcattpurh.sHtML

echo "${#arr[@]}"
来源：http://wap.fehbvm.com/Article/details/guzjqgncd.sHtML

[R20] 关联数组（字典）
来源：http://www.share.fehbvm.com/Article/details/gcaskfwwb.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.fehbvm.com/Article/details/gdrmaxucc.sHtML

[R21] 字符串长度
来源：http://baike.fehbvm.com/Article/details/gmslgexbn.sHtML

echo "${#s}"
来源：http://baike.hesvh.cn/Article/details/gjyxfuniu.sHtML

[R22] 截取子串
来源：http://www.m.share.hesvh.cn/Article/details/grsfvqqqs.sHtML

echo "${s:0:5}"
来源：http://blog.hesvh.cn/Article/details/gdvpsstrd.sHtML

[R23] 字符串替换
来源：http://mobile.hesvh.cn/Article/details/gjorjxzcw.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.fehbvm.com/Article/details/gyegdgsyd.sHtML

[R24] 大小写转换
来源：http://mobile.zdbjq.cn/Article/details/gpfpyyvnl.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fehbvm.com/Article/details/gzxqkgnyo.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fehbvm.com/Article/details/gtllbjokv.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.fehbvm.com/Article/details/gfsbolint.sHtML

[R26] 命令替换
来源：http://www.share.hesvh.cn/Article/details/gzvajbmic.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.hesvh.cn/Article/details/gteksjyzs.sHtML

[R27] 算术展开
来源：http://wap.hesvh.cn/Article/details/gqtqxenli.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.hesvh.cn/Article/details/gdzkvvstc.sHtML

[R28] 浮点运算
来源：http://blog.zdbjq.cn/Article/details/gwapooinv.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.fehbvm.com/Article/details/gnetzxhyk.sHtML

[R29] 定义函数
来源：http://m.share.fehbvm.com/Article/details/gqerezdyo.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.zdbjq.cn/Article/details/gvmqcoyhv.sHtML

[R30] 函数返回状态码
来源：http://m.share.fehbvm.com/Article/details/ghxqhmcpn.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.zdbjq.cn/Article/details/gprkpffit.sHtML

[R31] 局部变量
来源：http://mobile.fehbvm.com/Article/details/gejnwjonc.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.hesvh.cn/Article/details/gtjwamqha.sHtML

[R32] 参数个数校验
来源：http://blog.fehbvm.com/Article/details/gxgussfpb.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.hesvh.cn/Article/details/gdbxktjxs.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fehbvm.com/Article/details/gwaxiaicg.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.hesvh.cn/Article/details/gixkifmuw.sHtML

[R34] 退出时清理
来源：http://m.share.fehbvm.com/Article/details/gbitjhdvb.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fehbvm.com/Article/details/gmgsasfkv.sHtML

[R35] 后台执行并等待
来源：http://wap.zdbjq.cn/Article/details/ggzlkwmds.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.zdbjq.cn/Article/details/glfyptbxu.sHtML

[R36] 并发执行多个任务
来源：http://read.share.hesvh.cn/Article/details/gyflzcwfb.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.fehbvm.com/Article/details/gjtginopd.sHtML

[R37] 把输出赋给变量
来源：http://mobile.zdbjq.cn/Article/details/ghjdkngfq.sHtML

files=$(ls -1)
来源：http://baike.zdbjq.cn/Article/details/ghfzwasfb.sHtML

[R38] 管道串联
来源：http://www.share.hesvh.cn/Article/details/ghvvzhqvn.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.hesvh.cn/Article/details/gmohupzxe.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.zdbjq.cn/Article/details/gsuajnsrh.sHtML

cmd > out.log 2>&1
来源：http://read.share.zdbjq.cn/Article/details/gdaerfakc.sHtML

[R40] 追加写日志
来源：http://blog.hesvh.cn/Article/details/gxkawozdk.sHtML

echo "log" >> out.log
来源：http://read.share.fehbvm.com/Article/details/grizrgaiu.sHtML

[R41] 丢弃输出
来源：http://www.share.fehbvm.com/Article/details/gcjufzlho.sHtML

cmd >/dev/null 2>&1
来源：http://wap.hesvh.cn/Article/details/grnxikvxh.sHtML

[R42] 输入重定向
来源：http://3g.hesvh.cn/Article/details/glarcyxpf.sHtML

wc -l < a.txt
来源：http://baike.hesvh.cn/Article/details/gqgisjwig.sHtML

[R43] 按名字查找文件
来源：http://read.share.hesvh.cn/Article/details/gfkxlwrik.sHtML

find . -name "*.log" -type f
来源：http://baike.zdbjq.cn/Article/details/gismshjzt.sHtML

[R44] 按修改时间查找
来源：http://wap.fehbvm.com/Article/details/giqiwkron.sHtML

find . -mtime -7 -type f
来源：http://blog.zdbjq.cn/Article/details/grtbvighv.sHtML

[R45] 批量删除
来源：http://read.share.zdbjq.cn/Article/details/gnmtmhxcg.sHtML

find . -name "*.tmp" -delete
来源：http://3g.hesvh.cn/Article/details/gtvvitdvy.sHtML

[R46] 递归替换文件内容
来源：http://blog.fehbvm.com/Article/details/gbmrlpgtz.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fehbvm.com/Article/details/gwcveoioy.sHtML

[R47] sed 单行替换
来源：http://mobile.zdbjq.cn/Article/details/gnacpvwfq.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.fehbvm.com/Article/details/gtkxshyhx.sHtML

[R48] awk 取指定列
来源：http://read.share.hesvh.cn/Article/details/gmpvkdkbf.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.hesvh.cn/Article/details/ggnknplar.sHtML

[R49] awk 带条件
来源：http://wap.hesvh.cn/Article/details/grzixqvuf.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.zdbjq.cn/Article/details/gxcqffbtr.sHtML

[R50] awk 求和
来源：http://wap.hesvh.cn/Article/details/ggjsflnuw.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.hesvh.cn/Article/details/gftbstaww.sHtML

[R51] 排序去重取前几
来源：http://3g.fehbvm.com/Article/details/gjihxmomb.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.fehbvm.com/Article/details/grccxwudz.sHtML

[R52] 统计行数
来源：http://m.share.hesvh.cn/Article/details/gkxuysaeh.sHtML

wc -l a.txt
来源：http://read.share.zdbjq.cn/Article/details/griyfvdwg.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.zdbjq.cn/Article/details/gwrdesaxx.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.hesvh.cn/Article/details/gzkvqcocw.sHtML

[R54] 比较两个文件
来源：http://mobile.hesvh.cn/Article/details/gfxzfursp.sHtML

diff a.txt b.txt
来源：http://www.share.fehbvm.com/Article/details/gdfxxtfsk.sHtML

[R55] 压缩与解压
来源：http://3g.fehbvm.com/Article/details/gbtmhqljk.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fehbvm.com/Article/details/gguyrbtyq.sHtML

[R56] 远程拷贝
来源：http://m.share.zdbjq.cn/Article/details/gpndauuym.sHtML

scp file user@host:/path/
来源：http://www.share.fehbvm.com/Article/details/gfzijmgsl.sHtML

[R57] 远程执行命令
来源：http://3g.fehbvm.com/Article/details/gyuhxtrib.sHtML

ssh user@host 'uptime'
来源：http://blog.hesvh.cn/Article/details/gwchmwqak.sHtML

[R58] 下载文件
来源：http://baike.hesvh.cn/Article/details/gmpvglefg.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.fehbvm.com/Article/details/ghtphbumw.sHtML

[R59] 发 POST JSON
来源：http://blog.zdbjq.cn/Article/details/gipgavqph.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.hesvh.cn/Article/details/gscltmdyu.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.fehbvm.com/Article/details/gelryyxxm.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.zdbjq.cn/Article/details/gvjletglq.sHtML

[R61] 磁盘占用
来源：http://mobile.hesvh.cn/Article/details/gilgkomfi.sHtML

df -h;  du -sh *
来源：http://baike.fehbvm.com/Article/details/guyyroidb.sHtML

[R62] 找最占空间的文件
来源：http://www.share.zdbjq.cn/Article/details/gdlmktjrh.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.hesvh.cn/Article/details/gkmdxgcky.sHtML

[R63] 内存与进程
来源：http://3g.hesvh.cn/Article/details/gowvxwlux.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.hesvh.cn/Article/details/gqtikrjhq.sHtML

[R64] 结束进程
来源：http://www.share.fehbvm.com/Article/details/gslkdjpxz.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.zdbjq.cn/Article/details/gdwjdttxp.sHtML

[R65] 查看端口占用
来源：http://baike.hesvh.cn/Article/details/gwmhbhlht.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.hesvh.cn/Article/details/gwtmcauaa.sHtML

[R66] 定时任务
来源：http://3g.zdbjq.cn/Article/details/grvejugff.sHtML

crontab -e;  crontab -l
来源：http://m.share.fehbvm.com/Article/details/geosehhiq.sHtML

[R67] 生成随机十六进制串
来源：http://3g.zdbjq.cn/Article/details/gcoudlfmt.sHtML

openssl rand -hex 16
来源：http://www.share.zdbjq.cn/Article/details/glpioqmzr.sHtML

[R68] 计算文件校验值
来源：http://baike.fehbvm.com/Article/details/gfceogeuj.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.hesvh.cn/Article/details/gimhmaaxx.sHtML

[R69] 生成随机密码
来源：http://read.share.zdbjq.cn/Article/details/gmpzsfvyg.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fehbvm.com/Article/details/giurqvush.sHtML

[R70] 时间戳与互转
来源：http://blog.fehbvm.com/Article/details/gooxdngyc.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.zdbjq.cn/Article/details/gxkfyqubr.sHtML

[R71] 日期格式化
来源：http://wap.zdbjq.cn/Article/details/gdxxtsfbj.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fehbvm.com/Article/details/gvxeiolxf.sHtML

[R72] 等待端口就绪
来源：http://blog.zdbjq.cn/Article/details/gbnmsbqpi.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fehbvm.com/Article/details/gsrfkzdii.sHtML

[R73] 分割大日志
来源：http://www.share.fehbvm.com/Article/details/gomlfujho.sHtML

split -l 1000 big.log part_
来源：http://m.share.fehbvm.com/Article/details/gagryecbl.sHtML

[R74] 批量重命名
来源：http://m.share.hesvh.cn/Article/details/gumgpbalw.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fehbvm.com/Article/details/gaoocuerw.sHtML

[R75] 导出环境变量
来源：http://www.blog.zdbjq.cn/Article/details/gvobrwtqd.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.hesvh.cn/Article/details/gpvetxlwx.sHtML

[R76] 使用临时文件
来源：http://www.share.hesvh.cn/Article/details/goapcuctk.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fehbvm.com/Article/details/gjvuijuwc.sHtML

[R77] 读取用户输入
来源：http://www.share.hesvh.cn/Article/details/geyjfyjwf.sHtML

read -rp "请输入: " ans
来源：http://3g.zdbjq.cn/Article/details/gtrxkzdek.sHtML

[R78] 交互式菜单
来源：http://3g.zdbjq.cn/Article/details/gdtjgcfdq.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.hesvh.cn/Article/details/gykbueleb.sHtML

[R79] 解析命令行选项
来源：http://www.blog.fehbvm.com/Article/details/gyjgbdkrw.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.hesvh.cn/Article/details/gkbsbbbru.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.zdbjq.cn/Article/details/geqhlufkn.sHtML

time ./run.sh
来源：http://blog.fehbvm.com/Article/details/gvspctngy.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gkzsepome.sHtML

S. C / C++ 专题
来源：http://www.blog.fehbvm.com/Article/details/gxrhsgrkf.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gqfwfvonk.sHtML

[S01] C：Hello World
来源：http://blog.zdbjq.cn/Article/details/gschgdkno.sHtML

#include <stdio.h>
来源：http://www.m.share.fehbvm.com/Article/details/gdtqtunbh.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.zdbjq.cn/Article/details/gfzxfbzam.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.zdbjq.cn/Article/details/gajhjcxeg.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.hesvh.cn/Article/details/galtkbrtd.sHtML

[S03] C：读入整数
来源：http://wap.hesvh.cn/Article/details/ghvjvzdrg.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.zdbjq.cn/Article/details/giaxghvvg.sHtML

[S04] C：字符串复制
来源：http://www.blog.hesvh.cn/Article/details/gnvrayqpi.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.hesvh.cn/Article/details/glwhdzoys.sHtML

[S05] C：字符串长度
来源：http://baike.fehbvm.com/Article/details/gtbwzoocp.sHtML

strlen(s)
来源：http://wap.hesvh.cn/Article/details/gpsuiykuq.sHtML

[S06] C：字符串比较
来源：http://read.share.zdbjq.cn/Article/details/gyxctcwhk.sHtML

strcmp(a, b) == 0
来源：http://m.share.zdbjq.cn/Article/details/gpwqessjc.sHtML

[S07] C：数组遍历求和
来源：http://3g.zdbjq.cn/Article/details/gvqyeohqe.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.fehbvm.com/Article/details/gprrswqxk.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fehbvm.com/Article/details/gcytuqrgr.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.hesvh.cn/Article/details/gbhvgmqum.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.hesvh.cn/Article/details/gmboqhsgg.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.hesvh.cn/Article/details/grzqzrxkj.sHtML

[S10] C：指针与解引用
来源：http://baike.hesvh.cn/Article/details/gzjegohhu.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.fehbvm.com/Article/details/gqzabjdao.sHtML

[S11] C：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gkcvfrwvo.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.zdbjq.cn/Article/details/gewchmvkj.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.hesvh.cn/Article/details/goqgmojmm.sHtML

fclose(f);
来源：http://mobile.hesvh.cn/Article/details/gffkstrkh.sHtML

[S12] C：写文件
来源：http://www.blog.zdbjq.cn/Article/details/glqrgupwb.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.zdbjq.cn/Article/details/gwxowpuon.sHtML

[S13] C：宏定义
来源：http://baike.zdbjq.cn/Article/details/ganuoklrq.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.zdbjq.cn/Article/details/gftwbufvt.sHtML

[S14] C：枚举
来源：http://m.share.hesvh.cn/Article/details/gwdlxldvy.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.hesvh.cn/Article/details/gxcsptcqd.sHtML

[S15] C：类型转换
来源：http://baike.hesvh.cn/Article/details/gwtemfcce.sHtML

(double) a / b
来源：http://www.blog.fehbvm.com/Article/details/gjsurcbsj.sHtML

[S16] C：位操作置位
来源：http://www.blog.fehbvm.com/Article/details/gtifskfra.sHtML

x |= (1 << 3);
来源：http://m.share.fehbvm.com/Article/details/gmmvegdqf.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.hesvh.cn/Article/details/ghrkjkddp.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.hesvh.cn/Article/details/gjovlhnmd.sHtML

[S18] C：命令行参数
来源：http://www.m.share.hesvh.cn/Article/details/gougrkmkw.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fehbvm.com/Article/details/gtsanapih.sHtML

[S19] C：快速排序
来源：http://m.share.hesvh.cn/Article/details/gykyqtkyd.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fehbvm.com/Article/details/gjlaslgkd.sHtML

[S20] C：二分查找
来源：http://wap.zdbjq.cn/Article/details/ggvtbarjj.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/gcyljkwjg.sHtML

[S21] C：字符类别判断
来源：http://3g.zdbjq.cn/Article/details/gspgqskoe.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.zdbjq.cn/Article/details/gecajvznh.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.hesvh.cn/Article/details/gcmqwkmeo.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fehbvm.com/Article/details/ghooannmy.sHtML

[S23] C：随机数
来源：http://baike.zdbjq.cn/Article/details/gyeaygear.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.fehbvm.com/Article/details/gpzuxtsdd.sHtML

[S24] C：获取本地时间
来源：http://mobile.fehbvm.com/Article/details/gsxmzgmts.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.zdbjq.cn/Article/details/ghkmrrtnt.sHtML

[S25] C：内存拷贝
来源：http://baike.fehbvm.com/Article/details/gtoakrgdx.sHtML

memcpy(dst, src, n);
来源：http://wap.fehbvm.com/Article/details/gwjosauyv.sHtML

[S26] C：内存清零
来源：http://read.share.hesvh.cn/Article/details/gwnsptlky.sHtML

memset(a, 0, sizeof a);
来源：http://wap.zdbjq.cn/Article/details/gypfpsxqo.sHtML

[S27] C：定义常量
来源：http://read.share.fehbvm.com/Article/details/gjisvgxbq.sHtML

const double PI = 3.14159;
来源：http://3g.fehbvm.com/Article/details/ggmffmumi.sHtML

[S28] C：静态变量
来源：http://baike.hesvh.cn/Article/details/gcerdqrvh.sHtML

static int counter = 0;
来源：http://www.blog.zdbjq.cn/Article/details/ghlkvofgg.sHtML

[S29] C：变参函数
来源：http://wap.hesvh.cn/Article/details/gupwpnprk.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.zdbjq.cn/Article/details/gytquifpf.sHtML

[S30] C：头文件保护
来源：http://www.m.share.hesvh.cn/Article/details/gsfgdraox.sHtML

#ifndef X_H
来源：http://www.blog.fehbvm.com/Article/details/gzawljper.sHtML

#define X_H
来源：http://baike.zdbjq.cn/Article/details/gqhyxanyf.sHtML

#endif
来源：http://mobile.hesvh.cn/Article/details/gubgturps.sHtML

[S31] C++：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gozjjdrjh.sHtML

#include <iostream>
来源：http://m.share.zdbjq.cn/Article/details/goaodcnxi.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fehbvm.com/Article/details/ggscuwfmm.sHtML

[S32] C++：字符串
来源：http://m.share.hesvh.cn/Article/details/gairflfyz.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.fehbvm.com/Article/details/gbjdsethf.sHtML

[S33] C++：vector 增删
来源：http://mobile.fehbvm.com/Article/details/gxglckahz.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.zdbjq.cn/Article/details/gmbtxwwld.sHtML

[S34] C++：遍历 vector
来源：http://wap.fehbvm.com/Article/details/girzklkgs.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.zdbjq.cn/Article/details/gfmrwviwh.sHtML

[S35] C++：map
来源：http://www.share.zdbjq.cn/Article/details/genihdcqv.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fehbvm.com/Article/details/grroinhpl.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.zdbjq.cn/Article/details/gztabcyrx.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.hesvh.cn/Article/details/gmnseuzoh.sHtML

[S37] C++：set
来源：http://www.m.share.fehbvm.com/Article/details/gabwamjfq.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.hesvh.cn/Article/details/gqkroprlx.sHtML

[S38] C++：排序
来源：http://blog.fehbvm.com/Article/details/gaqwxtdow.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.zdbjq.cn/Article/details/gqbeysycn.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fehbvm.com/Article/details/gaznkmoof.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.hesvh.cn/Article/details/gseobdncs.sHtML

[S40] C++：查找元素
来源：http://3g.hesvh.cn/Article/details/grbzyjgfe.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.zdbjq.cn/Article/details/gokwxlkqa.sHtML

[S41] C++：类与构造函数
来源：http://blog.zdbjq.cn/Article/details/golofiyen.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.fehbvm.com/Article/details/gostcqkem.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.zdbjq.cn/Article/details/gtskumoqg.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.hesvh.cn/Article/details/gmwnzrsrt.sHtML


<!-- 参考信息 -->