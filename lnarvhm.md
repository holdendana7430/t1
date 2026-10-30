代发 wailian999

[Q76] 按天统计
来源：http://www.share.fehbvm.com/Article/details/gfsohfryb.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.hesvh.cn/Article/details/gcsikpljg.sHtML

[Q77] 时间加减
来源：http://blog.fehbvm.com/Article/details/gyhkzavjt.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.hesvh.cn/Article/details/grhvlxlqu.sHtML

[Q78] 当前时间
来源：http://mobile.zdbjq.cn/Article/details/ghywufgtb.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.hesvh.cn/Article/details/gxvvxhkks.sHtML

[Q79] 字符串拼接
来源：http://3g.hesvh.cn/Article/details/gtoplaarj.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.zdbjq.cn/Article/details/gejlcsoia.sHtML

[Q80] 字符串截取
来源：http://www.blog.fehbvm.com/Article/details/ggjqocjrf.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gwrvfjbho.sHtML

[Q81] 字符串替换
来源：http://baike.zdbjq.cn/Article/details/gqooitfco.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.zdbjq.cn/Article/details/glxrebezk.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.zdbjq.cn/Article/details/gdkhagvbo.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gdehpcldf.sHtML

[Q83] 大小写转换
来源：http://www.m.share.zdbjq.cn/Article/details/gozayocww.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/grthmobwq.sHtML

[Q84] 去除首尾空格
来源：http://www.share.zdbjq.cn/Article/details/gxxblkfzq.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gabanmwdu.sHtML

[Q85] 数值取整
来源：http://read.share.hesvh.cn/Article/details/gaudxwdnw.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.fehbvm.com/Article/details/gscracjwt.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.hesvh.cn/Article/details/gagvyzxkj.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.fehbvm.com/Article/details/gqwbwoohm.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.zdbjq.cn/Article/details/gkskodndu.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.zdbjq.cn/Article/details/gwhxwajwr.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.fehbvm.com/Article/details/gcdthlcun.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.zdbjq.cn/Article/details/ghzvfcyyq.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.fehbvm.com/Article/details/gyfitoxoy.sHtML

[Q89] 判断表是否存在
来源：http://www.share.hesvh.cn/Article/details/ggxphfrnv.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.fehbvm.com/Article/details/gopwigbfi.sHtML

[Q90] 生成序号列
来源：http://www.blog.zdbjq.cn/Article/details/gcxdequoo.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.fehbvm.com/Article/details/gyzgypiub.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gsgqwnirg.sHtML

R. Bash 专题
来源：http://www.m.share.zdbjq.cn/Article/details/gvwbkvvoo.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gmyrodwbd.sHtML

[R01] shebang 与严格模式
来源：http://m.share.fehbvm.com/Article/details/gtjyoansj.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.zdbjq.cn/Article/details/gqrguwbuy.sHtML

set -euo pipefail
来源：http://m.share.hesvh.cn/Article/details/gkzzgxbtk.sHtML

[R02] 变量赋值与使用
来源：http://mobile.hesvh.cn/Article/details/gdxbcqomz.sHtML

name="Tom"; echo "$name"
来源：http://read.share.zdbjq.cn/Article/details/gnmjxkqyb.sHtML

[R03] 只读变量
来源：http://www.blog.zdbjq.cn/Article/details/gqaqxsiav.sHtML

readonly PI=3.14
来源：http://baike.hesvh.cn/Article/details/ginjqdrhu.sHtML

[R04] 位置参数
来源：http://www.blog.zdbjq.cn/Article/details/ghklpgtis.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.zdbjq.cn/Article/details/gboesytiz.sHtML

[R05] 参数默认值
来源：http://3g.zdbjq.cn/Article/details/gdxaxkfxp.sHtML

name="${1:-default}"
来源：http://wap.zdbjq.cn/Article/details/giepqmdlo.sHtML

[R06] 判断命令是否存在
来源：http://3g.zdbjq.cn/Article/details/ghdqztsam.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.fehbvm.com/Article/details/gblupxcuc.sHtML

[R07] if 判断文件
来源：http://read.share.fehbvm.com/Article/details/gibauvibi.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.hesvh.cn/Article/details/gtlxnfots.sHtML

[R08] 数值比较
来源：http://baike.hesvh.cn/Article/details/goydhyiix.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.fehbvm.com/Article/details/gczlxeoce.sHtML

[R09] 字符串比较
来源：http://wap.zdbjq.cn/Article/details/gyhyjjtqt.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.fehbvm.com/Article/details/gjzvuhyba.sHtML

[R10] 正则匹配
来源：http://baike.zdbjq.cn/Article/details/gjeiunbdc.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.fehbvm.com/Article/details/gwxgmhwdb.sHtML

[R11] case 多分支
来源：http://mobile.hesvh.cn/Article/details/gmrgvbptv.sHtML

case "$1" in
来源：http://mobile.hesvh.cn/Article/details/goiyuhygm.sHtML

start) echo "启动" ;;
来源：http://blog.fehbvm.com/Article/details/gsynvqxdv.sHtML

stop)  echo "停止" ;;
来源：http://m.share.hesvh.cn/Article/details/gscedbqnr.sHtML

*)     echo "未知命令" ;;
来源：http://blog.zdbjq.cn/Article/details/gnfldqfov.sHtML

esac
来源：http://baike.fehbvm.com/Article/details/gahnqpgll.sHtML

[R12] for 遍历文件
来源：http://wap.zdbjq.cn/Article/details/gxjmlomrk.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.zdbjq.cn/Article/details/gnqotrdtp.sHtML

[R13] for 计数循环
来源：http://blog.fehbvm.com/Article/details/grewjjebb.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.zdbjq.cn/Article/details/gymmrmjtq.sHtML

[R14] C 风格 for
来源：http://blog.zdbjq.cn/Article/details/gxoetgjdv.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.zdbjq.cn/Article/details/gvhrgfrrw.sHtML

[R15] while 逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gzdnwdgku.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.hesvh.cn/Article/details/ghzpxzawh.sHtML

[R16] until 等待条件
来源：http://wap.zdbjq.cn/Article/details/gnxcmaxdy.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fehbvm.com/Article/details/gyeuxkprm.sHtML

[R17] 数组定义与取值
来源：http://baike.zdbjq.cn/Article/details/gkeyximoc.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.zdbjq.cn/Article/details/gfgstbxfj.sHtML

[R18] 遍历数组
来源：http://read.share.zdbjq.cn/Article/details/ghftyovsd.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.zdbjq.cn/Article/details/gzwxqkruc.sHtML

[R19] 数组长度
来源：http://m.share.hesvh.cn/Article/details/gptzgmfoi.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.fehbvm.com/Article/details/gjdpkturz.sHtML

[R20] 关联数组（字典）
来源：http://wap.hesvh.cn/Article/details/gmirmdfds.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.hesvh.cn/Article/details/gqjekutfz.sHtML

[R21] 字符串长度
来源：http://mobile.fehbvm.com/Article/details/gfwstfluq.sHtML

echo "${#s}"
来源：http://baike.zdbjq.cn/Article/details/gmfynmpua.sHtML

[R22] 截取子串
来源：http://mobile.fehbvm.com/Article/details/gahthzkzh.sHtML

echo "${s:0:5}"
来源：http://wap.zdbjq.cn/Article/details/gvsrrunkt.sHtML

[R23] 字符串替换
来源：http://m.share.zdbjq.cn/Article/details/gdrotukgl.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.fehbvm.com/Article/details/gfaqytubg.sHtML

[R24] 大小写转换
来源：http://blog.zdbjq.cn/Article/details/gexrvxgsk.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.zdbjq.cn/Article/details/gfoxjnirp.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.fehbvm.com/Article/details/gvuxczsem.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.hesvh.cn/Article/details/gzmxddcud.sHtML

[R26] 命令替换
来源：http://blog.zdbjq.cn/Article/details/gyhwukqcb.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.fehbvm.com/Article/details/gqmlogche.sHtML

[R27] 算术展开
来源：http://www.share.zdbjq.cn/Article/details/gdsffeptw.sHtML

echo $((1 + 2 * 3))
来源：http://3g.fehbvm.com/Article/details/geqfyqizm.sHtML

[R28] 浮点运算
来源：http://www.m.share.zdbjq.cn/Article/details/gkgfipbhe.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fehbvm.com/Article/details/gidpyscfh.sHtML

[R29] 定义函数
来源：http://www.share.fehbvm.com/Article/details/gqoktoebs.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.zdbjq.cn/Article/details/gkuinzveh.sHtML

[R30] 函数返回状态码
来源：http://www.share.fehbvm.com/Article/details/gemcvnswn.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.zdbjq.cn/Article/details/gmypnvofe.sHtML

[R31] 局部变量
来源：http://baike.hesvh.cn/Article/details/gqrraignl.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.hesvh.cn/Article/details/gzwvunnhl.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fehbvm.com/Article/details/gyftwaujc.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.fehbvm.com/Article/details/gizjbzjpk.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.fehbvm.com/Article/details/gfsvcmgcx.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.zdbjq.cn/Article/details/gdayglqhs.sHtML

[R34] 退出时清理
来源：http://baike.fehbvm.com/Article/details/gcweqosud.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.fehbvm.com/Article/details/gvhcozalf.sHtML

[R35] 后台执行并等待
来源：http://read.share.fehbvm.com/Article/details/gmtijbpnx.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fehbvm.com/Article/details/gwhswdgel.sHtML

[R36] 并发执行多个任务
来源：http://3g.fehbvm.com/Article/details/gvafqmflu.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.zdbjq.cn/Article/details/gbhjefwla.sHtML

[R37] 把输出赋给变量
来源：http://read.share.fehbvm.com/Article/details/gwwnjwxnt.sHtML

files=$(ls -1)
来源：http://www.m.share.fehbvm.com/Article/details/gxkfnqjir.sHtML

[R38] 管道串联
来源：http://wap.fehbvm.com/Article/details/gftjoyudw.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.hesvh.cn/Article/details/gxbhxxfts.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.hesvh.cn/Article/details/grsfpdmod.sHtML

cmd > out.log 2>&1
来源：http://blog.fehbvm.com/Article/details/gocefzuay.sHtML

[R40] 追加写日志
来源：http://wap.hesvh.cn/Article/details/gtnmatzyz.sHtML

echo "log" >> out.log
来源：http://blog.fehbvm.com/Article/details/gwsfczfff.sHtML

[R41] 丢弃输出
来源：http://3g.fehbvm.com/Article/details/ghlprvpmt.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fehbvm.com/Article/details/ggdxwtxhu.sHtML

[R42] 输入重定向
来源：http://www.blog.fehbvm.com/Article/details/glxizkfqm.sHtML

wc -l < a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gyaqxlizs.sHtML

[R43] 按名字查找文件
来源：http://mobile.hesvh.cn/Article/details/gzgtyigxy.sHtML

find . -name "*.log" -type f
来源：http://3g.fehbvm.com/Article/details/gzccyfymt.sHtML

[R44] 按修改时间查找
来源：http://baike.fehbvm.com/Article/details/gesvhweyr.sHtML

find . -mtime -7 -type f
来源：http://www.share.zdbjq.cn/Article/details/gznwpdzzu.sHtML

[R45] 批量删除
来源：http://www.share.hesvh.cn/Article/details/gvkjfuxju.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fehbvm.com/Article/details/geslhsqgi.sHtML

[R46] 递归替换文件内容
来源：http://www.share.fehbvm.com/Article/details/grsugcyrp.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.hesvh.cn/Article/details/gmqrxspya.sHtML

[R47] sed 单行替换
来源：http://www.blog.hesvh.cn/Article/details/gzcbourpp.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.hesvh.cn/Article/details/gxbvgascu.sHtML

[R48] awk 取指定列
来源：http://3g.hesvh.cn/Article/details/gbuhhikci.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.zdbjq.cn/Article/details/gpdjezmff.sHtML

[R49] awk 带条件
来源：http://baike.fehbvm.com/Article/details/gzdbewycb.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.hesvh.cn/Article/details/gpdbhyyiz.sHtML

[R50] awk 求和
来源：http://3g.fehbvm.com/Article/details/goggqttya.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.hesvh.cn/Article/details/gzajpgyqm.sHtML

[R51] 排序去重取前几
来源：http://m.share.fehbvm.com/Article/details/gqjcxwzwb.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.hesvh.cn/Article/details/ggioweepa.sHtML

[R52] 统计行数
来源：http://baike.zdbjq.cn/Article/details/gsmyjezxm.sHtML

wc -l a.txt
来源：http://blog.fehbvm.com/Article/details/ghkzrsqnd.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fehbvm.com/Article/details/glapgzooi.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.zdbjq.cn/Article/details/gbsibjkhj.sHtML

[R54] 比较两个文件
来源：http://3g.hesvh.cn/Article/details/gdsdveqva.sHtML

diff a.txt b.txt
来源：http://mobile.hesvh.cn/Article/details/gfhtnydpv.sHtML

[R55] 压缩与解压
来源：http://blog.fehbvm.com/Article/details/gkciunpfp.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.zdbjq.cn/Article/details/gfybznfjf.sHtML

[R56] 远程拷贝
来源：http://www.m.share.fehbvm.com/Article/details/gbuioxtvh.sHtML

scp file user@host:/path/
来源：http://mobile.hesvh.cn/Article/details/glwrmjkrh.sHtML

[R57] 远程执行命令
来源：http://www.blog.hesvh.cn/Article/details/gvectymal.sHtML

ssh user@host 'uptime'
来源：http://www.share.hesvh.cn/Article/details/grmdnrkel.sHtML

[R58] 下载文件
来源：http://blog.fehbvm.com/Article/details/gyynqgwoc.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.zdbjq.cn/Article/details/gqbrzmaxr.sHtML

[R59] 发 POST JSON
来源：http://blog.zdbjq.cn/Article/details/gtmvxwkkx.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.hesvh.cn/Article/details/gfxqpqqkm.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fehbvm.com/Article/details/gwsqbohfs.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.zdbjq.cn/Article/details/gbadzdvze.sHtML

[R61] 磁盘占用
来源：http://m.share.zdbjq.cn/Article/details/gprwtnyxt.sHtML

df -h;  du -sh *
来源：http://blog.hesvh.cn/Article/details/gzsemskap.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.fehbvm.com/Article/details/gildrognl.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.fehbvm.com/Article/details/gnvgtljhr.sHtML

[R63] 内存与进程
来源：http://mobile.hesvh.cn/Article/details/gxkhnogzy.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.fehbvm.com/Article/details/gejpubitn.sHtML

[R64] 结束进程
来源：http://www.share.fehbvm.com/Article/details/gmtcpeawl.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.zdbjq.cn/Article/details/gnjklrbig.sHtML

[R65] 查看端口占用
来源：http://m.share.fehbvm.com/Article/details/genyluzcd.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.zdbjq.cn/Article/details/gnrgnnsmo.sHtML

[R66] 定时任务
来源：http://blog.zdbjq.cn/Article/details/gouyfjhsz.sHtML

crontab -e;  crontab -l
来源：http://mobile.fehbvm.com/Article/details/gjnorwznc.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.zdbjq.cn/Article/details/glnliinls.sHtML

openssl rand -hex 16
来源：http://m.share.zdbjq.cn/Article/details/ggpenilgn.sHtML

[R68] 计算文件校验值
来源：http://www.blog.zdbjq.cn/Article/details/gptcortcf.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.hesvh.cn/Article/details/ghpdkhylm.sHtML

[R69] 生成随机密码
来源：http://3g.fehbvm.com/Article/details/gcxwueseh.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fehbvm.com/Article/details/gaatzturm.sHtML

[R70] 时间戳与互转
来源：http://wap.hesvh.cn/Article/details/gheqnalot.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.hesvh.cn/Article/details/ghqzlgrsq.sHtML

[R71] 日期格式化
来源：http://wap.zdbjq.cn/Article/details/gvcfoqgqd.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.hesvh.cn/Article/details/gxtcszcyl.sHtML

[R72] 等待端口就绪
来源：http://baike.hesvh.cn/Article/details/gzrziinlw.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.zdbjq.cn/Article/details/ghscvmdok.sHtML

[R73] 分割大日志
来源：http://baike.zdbjq.cn/Article/details/gncdggoxq.sHtML

split -l 1000 big.log part_
来源：http://mobile.zdbjq.cn/Article/details/gvdoglcla.sHtML

[R74] 批量重命名
来源：http://wap.hesvh.cn/Article/details/ghglkrakr.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fehbvm.com/Article/details/ggihffepr.sHtML

[R75] 导出环境变量
来源：http://3g.hesvh.cn/Article/details/gbjpehtoe.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.zdbjq.cn/Article/details/gwcfjwmxk.sHtML

[R76] 使用临时文件
来源：http://3g.fehbvm.com/Article/details/gyqseshqe.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.hesvh.cn/Article/details/gvdxemamh.sHtML

[R77] 读取用户输入
来源：http://www.share.hesvh.cn/Article/details/ggrbgrguj.sHtML

read -rp "请输入: " ans
来源：http://www.share.zdbjq.cn/Article/details/gntqpzpig.sHtML

[R78] 交互式菜单
来源：http://blog.hesvh.cn/Article/details/gofjuqwkj.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.fehbvm.com/Article/details/gbmukaesw.sHtML

[R79] 解析命令行选项
来源：http://m.share.fehbvm.com/Article/details/geuwjojik.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.hesvh.cn/Article/details/gwszhznji.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.hesvh.cn/Article/details/gayqioghv.sHtML

time ./run.sh
来源：http://wap.fehbvm.com/Article/details/gwozwlwcw.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gfamkmkpe.sHtML

S. C / C++ 专题
来源：http://blog.fehbvm.com/Article/details/gtathktat.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gtgxefhis.sHtML

[S01] C：Hello World
来源：http://baike.hesvh.cn/Article/details/gzvyozqab.sHtML

#include <stdio.h>
来源：http://wap.fehbvm.com/Article/details/gfcgblckj.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.zdbjq.cn/Article/details/glidttjgk.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fehbvm.com/Article/details/gaasxfpry.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.hesvh.cn/Article/details/gpvgrtzws.sHtML

[S03] C：读入整数
来源：http://mobile.hesvh.cn/Article/details/gbldpkuou.sHtML

int x; scanf("%d", &x);
来源：http://mobile.zdbjq.cn/Article/details/gjepowmxy.sHtML

[S04] C：字符串复制
来源：http://www.share.fehbvm.com/Article/details/gtdubltyx.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fehbvm.com/Article/details/gytfnsitp.sHtML

[S05] C：字符串长度
来源：http://baike.zdbjq.cn/Article/details/gddoruqlx.sHtML

strlen(s)
来源：http://wap.zdbjq.cn/Article/details/gyagckaul.sHtML

[S06] C：字符串比较
来源：http://read.share.hesvh.cn/Article/details/guerrxnsh.sHtML

strcmp(a, b) == 0
来源：http://mobile.hesvh.cn/Article/details/guwiohxvf.sHtML

[S07] C：数组遍历求和
来源：http://m.share.zdbjq.cn/Article/details/ggsaadfdi.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.hesvh.cn/Article/details/gwbdspnhy.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.zdbjq.cn/Article/details/gztjgcmak.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.hesvh.cn/Article/details/gjeaolzcm.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.hesvh.cn/Article/details/goczjnnia.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.fehbvm.com/Article/details/gihhafzpt.sHtML

[S10] C：指针与解引用
来源：http://mobile.hesvh.cn/Article/details/gjgnpplja.sHtML

int *p = &a;  *p = 5;
来源：http://3g.fehbvm.com/Article/details/gxeztgmbn.sHtML

[S11] C：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gclupdart.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.zdbjq.cn/Article/details/gudhvtrwl.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fehbvm.com/Article/details/gjoyenivj.sHtML

fclose(f);
来源：http://www.blog.zdbjq.cn/Article/details/gzmxjwspa.sHtML

[S12] C：写文件
来源：http://www.blog.hesvh.cn/Article/details/gzvjlgoyb.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.hesvh.cn/Article/details/gickjrsra.sHtML

[S13] C：宏定义
来源：http://m.share.zdbjq.cn/Article/details/gkdgvkbih.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.fehbvm.com/Article/details/gmvaomkwo.sHtML

[S14] C：枚举
来源：http://www.blog.hesvh.cn/Article/details/ggjimlqwz.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.zdbjq.cn/Article/details/gcqxncnvr.sHtML

[S15] C：类型转换
来源：http://m.share.zdbjq.cn/Article/details/gwdmeeeco.sHtML

(double) a / b
来源：http://mobile.fehbvm.com/Article/details/gzoxbeyxn.sHtML

[S16] C：位操作置位
来源：http://www.blog.hesvh.cn/Article/details/gjunawxkg.sHtML

x |= (1 << 3);
来源：http://read.share.fehbvm.com/Article/details/gyrewenic.sHtML

[S17] C：安全拼接字符串
来源：http://baike.zdbjq.cn/Article/details/gbbhpsmmg.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.zdbjq.cn/Article/details/gmcjecxfq.sHtML

[S18] C：命令行参数
来源：http://wap.zdbjq.cn/Article/details/ghegmgzgh.sHtML

int main(int argc, char **argv)
来源：http://m.share.zdbjq.cn/Article/details/gftulkubq.sHtML

[S19] C：快速排序
来源：http://3g.hesvh.cn/Article/details/guirgtbsc.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.fehbvm.com/Article/details/gkanvuxqo.sHtML

[S20] C：二分查找
来源：http://3g.fehbvm.com/Article/details/gveomqost.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.hesvh.cn/Article/details/gyaphnmgx.sHtML

[S21] C：字符类别判断
来源：http://www.share.hesvh.cn/Article/details/gbypypgno.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fehbvm.com/Article/details/gcxhdnzxn.sHtML

[S22] C：字符串转数字
来源：http://mobile.fehbvm.com/Article/details/gjnpwicst.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.zdbjq.cn/Article/details/gwdhvklxp.sHtML

[S23] C：随机数
来源：http://baike.hesvh.cn/Article/details/gbdvkqopf.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.hesvh.cn/Article/details/gztpzpshe.sHtML

[S24] C：获取本地时间
来源：http://3g.fehbvm.com/Article/details/gmckrjvwb.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fehbvm.com/Article/details/gvssxuwgo.sHtML

[S25] C：内存拷贝
来源：http://m.share.fehbvm.com/Article/details/gctamlunv.sHtML

memcpy(dst, src, n);
来源：http://blog.fehbvm.com/Article/details/gfdtikqnz.sHtML

[S26] C：内存清零
来源：http://www.blog.zdbjq.cn/Article/details/gpxpifhkc.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.hesvh.cn/Article/details/gjfmxmcgb.sHtML

[S27] C：定义常量
来源：http://blog.hesvh.cn/Article/details/gmypzjiaj.sHtML

const double PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/grttxqxws.sHtML

[S28] C：静态变量
来源：http://mobile.fehbvm.com/Article/details/gpwntwqbx.sHtML

static int counter = 0;
来源：http://www.blog.zdbjq.cn/Article/details/gfjjhlhbm.sHtML

[S29] C：变参函数
来源：http://www.blog.fehbvm.com/Article/details/gbrirvvrm.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.hesvh.cn/Article/details/gpcvhdzbr.sHtML

[S30] C：头文件保护
来源：http://www.share.zdbjq.cn/Article/details/ghhwjwqrf.sHtML

#ifndef X_H
来源：http://read.share.hesvh.cn/Article/details/gkkvzmqit.sHtML

#define X_H
来源：http://3g.zdbjq.cn/Article/details/gjjdgaorm.sHtML

#endif
来源：http://mobile.fehbvm.com/Article/details/gzyhwddeg.sHtML

[S31] C++：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gguylocvw.sHtML

#include <iostream>
来源：http://3g.fehbvm.com/Article/details/gdxjfotmd.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.zdbjq.cn/Article/details/geieptxnc.sHtML

[S32] C++：字符串
来源：http://3g.hesvh.cn/Article/details/ghuupxinv.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.hesvh.cn/Article/details/gapjabqpo.sHtML

[S33] C++：vector 增删
来源：http://m.share.hesvh.cn/Article/details/gtbxphdun.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.hesvh.cn/Article/details/gimmfkixm.sHtML

[S34] C++：遍历 vector
来源：http://www.share.zdbjq.cn/Article/details/gwdzjruye.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.zdbjq.cn/Article/details/gpczsmzzz.sHtML

[S35] C++：map
来源：http://wap.hesvh.cn/Article/details/guqezmgtv.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/geowpvdjk.sHtML

[S36] C++：unordered_map
来源：http://m.share.fehbvm.com/Article/details/gfexjenkc.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/geovkgfid.sHtML

[S37] C++：set
来源：http://blog.fehbvm.com/Article/details/gtkslpitx.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fehbvm.com/Article/details/giztsyzuz.sHtML

[S38] C++：排序
来源：http://www.m.share.zdbjq.cn/Article/details/ghmsyubdi.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.zdbjq.cn/Article/details/ghivarcrf.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.zdbjq.cn/Article/details/gpbaijsre.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.zdbjq.cn/Article/details/gnljhnmoc.sHtML

[S40] C++：查找元素
来源：http://read.share.zdbjq.cn/Article/details/gztzghdiu.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.fehbvm.com/Article/details/gfpunwoif.sHtML

[S41] C++：类与构造函数
来源：http://mobile.zdbjq.cn/Article/details/gacvsfzxg.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.zdbjq.cn/Article/details/gikhvacee.sHtML

[S42] C++：继承与虚函数
来源：http://baike.hesvh.cn/Article/details/gqomcpiqy.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.zdbjq.cn/Article/details/ggttphima.sHtML

[S43] C++：智能指针
来源：http://3g.fehbvm.com/Article/details/gvsukfuzv.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.hesvh.cn/Article/details/gyicijidy.sHtML

[S44] C++：引用传参
来源：http://m.share.hesvh.cn/Article/details/gxtxmaesf.sHtML

void inc(int &x) { ++x; }
来源：http://3g.zdbjq.cn/Article/details/gfiezaziw.sHtML

[S45] C++：lambda
来源：http://m.share.hesvh.cn/Article/details/gkqebscaa.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.hesvh.cn/Article/details/gqkrsjylr.sHtML

[S46] C++：函数模板
来源：http://www.blog.fehbvm.com/Article/details/gbdgaswjn.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.zdbjq.cn/Article/details/giuqichhe.sHtML


<!-- 参考信息 -->