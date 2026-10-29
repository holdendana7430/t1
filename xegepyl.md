代发 wailian999

[Q76] 按天统计
来源：http://www.share.zdbjq.cn/Article/details/grazdsrio.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.hesvh.cn/Article/details/gqcyoojpp.sHtML

[Q77] 时间加减
来源：http://read.share.fehbvm.com/Article/details/gfwktfjkf.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.zdbjq.cn/Article/details/gpewoivnw.sHtML

[Q78] 当前时间
来源：http://m.share.hesvh.cn/Article/details/gikzhqosg.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.fehbvm.com/Article/details/goyzeodva.sHtML

[Q79] 字符串拼接
来源：http://baike.zdbjq.cn/Article/details/geoshurlc.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.fehbvm.com/Article/details/gszledvss.sHtML

[Q80] 字符串截取
来源：http://baike.hesvh.cn/Article/details/gsbggrzwd.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.hesvh.cn/Article/details/gocpgcvac.sHtML

[Q81] 字符串替换
来源：http://www.blog.zdbjq.cn/Article/details/gunjtkqfg.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.zdbjq.cn/Article/details/grjrgupbz.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.hesvh.cn/Article/details/gbbhlohww.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/gxdsmazcv.sHtML

[Q83] 大小写转换
来源：http://wap.fehbvm.com/Article/details/gyaxlqfte.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gandahlli.sHtML

[Q84] 去除首尾空格
来源：http://mobile.zdbjq.cn/Article/details/ggsieuitz.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.hesvh.cn/Article/details/gpwhntqqu.sHtML

[Q85] 数值取整
来源：http://mobile.zdbjq.cn/Article/details/grvpxeaau.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.fehbvm.com/Article/details/geqgvfyqi.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.hesvh.cn/Article/details/gjhpeppfq.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.zdbjq.cn/Article/details/gakmxwxqi.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.hesvh.cn/Article/details/ggwvkwudl.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.zdbjq.cn/Article/details/gfruwmzwv.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.fehbvm.com/Article/details/geigmqphn.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.zdbjq.cn/Article/details/grhudcmay.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gnstvhzmp.sHtML

[Q89] 判断表是否存在
来源：http://3g.fehbvm.com/Article/details/geitnppmk.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.fehbvm.com/Article/details/gzlmjszft.sHtML

[Q90] 生成序号列
来源：http://www.blog.hesvh.cn/Article/details/gwrkjfupg.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.zdbjq.cn/Article/details/gcdxbdjki.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/geuqrmein.sHtML

R. Bash 专题
来源：http://baike.fehbvm.com/Article/details/gfddnbalb.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/glbnnrcze.sHtML

[R01] shebang 与严格模式
来源：http://3g.zdbjq.cn/Article/details/gvxrlsyye.sHtML

#!/usr/bin/env bash
来源：http://mobile.fehbvm.com/Article/details/gruknqpoh.sHtML

set -euo pipefail
来源：http://mobile.zdbjq.cn/Article/details/gcphopeva.sHtML

[R02] 变量赋值与使用
来源：http://read.share.hesvh.cn/Article/details/gvykuqwno.sHtML

name="Tom"; echo "$name"
来源：http://blog.zdbjq.cn/Article/details/gkabszuhc.sHtML

[R03] 只读变量
来源：http://mobile.zdbjq.cn/Article/details/gluafhhdb.sHtML

readonly PI=3.14
来源：http://www.m.share.fehbvm.com/Article/details/gcqfrovjs.sHtML

[R04] 位置参数
来源：http://read.share.zdbjq.cn/Article/details/gygwkopoe.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.hesvh.cn/Article/details/gzmeucqgw.sHtML

[R05] 参数默认值
来源：http://read.share.fehbvm.com/Article/details/gccvvetiq.sHtML

name="${1:-default}"
来源：http://www.m.share.fehbvm.com/Article/details/gdijxxyvk.sHtML

[R06] 判断命令是否存在
来源：http://read.share.zdbjq.cn/Article/details/gdfiiajca.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.fehbvm.com/Article/details/gvfldfpqr.sHtML

[R07] if 判断文件
来源：http://read.share.zdbjq.cn/Article/details/gxaptcoun.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.fehbvm.com/Article/details/guqjuagrn.sHtML

[R08] 数值比较
来源：http://mobile.fehbvm.com/Article/details/gijncndcm.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.zdbjq.cn/Article/details/gehldaynb.sHtML

[R09] 字符串比较
来源：http://www.m.share.zdbjq.cn/Article/details/glsuzpnhr.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.hesvh.cn/Article/details/ggoqpjjae.sHtML

[R10] 正则匹配
来源：http://wap.zdbjq.cn/Article/details/gphkcdkuh.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.zdbjq.cn/Article/details/gpenkuros.sHtML

[R11] case 多分支
来源：http://3g.zdbjq.cn/Article/details/gmhshyqer.sHtML

case "$1" in
来源：http://wap.zdbjq.cn/Article/details/ggjmksbqw.sHtML

start) echo "启动" ;;
来源：http://mobile.zdbjq.cn/Article/details/gdscqnhlz.sHtML

stop)  echo "停止" ;;
来源：http://3g.zdbjq.cn/Article/details/gbuqxbudp.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.hesvh.cn/Article/details/gcegvpckx.sHtML

esac
来源：http://baike.hesvh.cn/Article/details/gtzofvolj.sHtML

[R12] for 遍历文件
来源：http://m.share.fehbvm.com/Article/details/gxxaeffqt.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.fehbvm.com/Article/details/gfictigrm.sHtML

[R13] for 计数循环
来源：http://wap.hesvh.cn/Article/details/gptgmwptw.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.hesvh.cn/Article/details/ghmkqpbgf.sHtML

[R14] C 风格 for
来源：http://read.share.hesvh.cn/Article/details/gsfqnpoud.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.fehbvm.com/Article/details/gexugcrcy.sHtML

[R15] while 逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gbplcvequ.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.fehbvm.com/Article/details/ghfszavqa.sHtML

[R16] until 等待条件
来源：http://m.share.hesvh.cn/Article/details/gwjyvmfrp.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fehbvm.com/Article/details/gmkrvxhqy.sHtML

[R17] 数组定义与取值
来源：http://wap.fehbvm.com/Article/details/gmzjisfqr.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.hesvh.cn/Article/details/gnwbpftcv.sHtML

[R18] 遍历数组
来源：http://wap.fehbvm.com/Article/details/gqlfvaioc.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.hesvh.cn/Article/details/gpliwzacm.sHtML

[R19] 数组长度
来源：http://www.blog.fehbvm.com/Article/details/ghmqtjfkx.sHtML

echo "${#arr[@]}"
来源：http://wap.fehbvm.com/Article/details/gillaquwa.sHtML

[R20] 关联数组（字典）
来源：http://read.share.hesvh.cn/Article/details/gqxwwjvuy.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.fehbvm.com/Article/details/gfjahtigr.sHtML

[R21] 字符串长度
来源：http://blog.fehbvm.com/Article/details/gqrhbvqto.sHtML

echo "${#s}"
来源：http://3g.fehbvm.com/Article/details/grxyabvzp.sHtML

[R22] 截取子串
来源：http://www.blog.zdbjq.cn/Article/details/gabhyaide.sHtML

echo "${s:0:5}"
来源：http://baike.hesvh.cn/Article/details/gnkxvwrhb.sHtML

[R23] 字符串替换
来源：http://wap.zdbjq.cn/Article/details/gxwshwjjk.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.hesvh.cn/Article/details/gxydhmtld.sHtML

[R24] 大小写转换
来源：http://m.share.zdbjq.cn/Article/details/ggbqjhgom.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.zdbjq.cn/Article/details/gexlfjxjl.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.fehbvm.com/Article/details/gfclampbc.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.hesvh.cn/Article/details/gtnvubaht.sHtML

[R26] 命令替换
来源：http://www.blog.zdbjq.cn/Article/details/glrwthxpe.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.zdbjq.cn/Article/details/godczjgfq.sHtML

[R27] 算术展开
来源：http://mobile.fehbvm.com/Article/details/gcpovlpah.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.zdbjq.cn/Article/details/gummybuvf.sHtML

[R28] 浮点运算
来源：http://read.share.hesvh.cn/Article/details/guenhpaoi.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.zdbjq.cn/Article/details/gqtmgvwik.sHtML

[R29] 定义函数
来源：http://baike.zdbjq.cn/Article/details/gojldtmeq.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.zdbjq.cn/Article/details/gqkctswnn.sHtML

[R30] 函数返回状态码
来源：http://blog.hesvh.cn/Article/details/gyxdvpxgy.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.hesvh.cn/Article/details/gboqucpln.sHtML

[R31] 局部变量
来源：http://baike.hesvh.cn/Article/details/gfwidzxft.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.hesvh.cn/Article/details/ggcmaswpq.sHtML

[R32] 参数个数校验
来源：http://blog.zdbjq.cn/Article/details/gatwjpxtw.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.hesvh.cn/Article/details/grecfztws.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.hesvh.cn/Article/details/gbiroshep.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.zdbjq.cn/Article/details/gsujefglv.sHtML

[R34] 退出时清理
来源：http://wap.hesvh.cn/Article/details/glpvxuypl.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.zdbjq.cn/Article/details/gamqbljjv.sHtML

[R35] 后台执行并等待
来源：http://www.share.fehbvm.com/Article/details/gkuwznyyz.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.hesvh.cn/Article/details/gxgyktkut.sHtML

[R36] 并发执行多个任务
来源：http://www.share.hesvh.cn/Article/details/gubtaoshv.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.zdbjq.cn/Article/details/gfnabuzxs.sHtML

[R37] 把输出赋给变量
来源：http://wap.hesvh.cn/Article/details/grjfyodes.sHtML

files=$(ls -1)
来源：http://wap.fehbvm.com/Article/details/gtcafixfq.sHtML

[R38] 管道串联
来源：http://mobile.fehbvm.com/Article/details/gggqmdgyz.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.hesvh.cn/Article/details/gbbhmasao.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.zdbjq.cn/Article/details/gfrzwzcib.sHtML

cmd > out.log 2>&1
来源：http://m.share.hesvh.cn/Article/details/glxytddaa.sHtML

[R40] 追加写日志
来源：http://www.share.hesvh.cn/Article/details/gbdlyvnjh.sHtML

echo "log" >> out.log
来源：http://blog.fehbvm.com/Article/details/goabjddlf.sHtML

[R41] 丢弃输出
来源：http://www.share.fehbvm.com/Article/details/gljyirwsm.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.hesvh.cn/Article/details/gyzgtkjqv.sHtML

[R42] 输入重定向
来源：http://mobile.zdbjq.cn/Article/details/gvhvkmtfe.sHtML

wc -l < a.txt
来源：http://wap.zdbjq.cn/Article/details/gytwslkno.sHtML

[R43] 按名字查找文件
来源：http://3g.zdbjq.cn/Article/details/gtjrquomv.sHtML

find . -name "*.log" -type f
来源：http://wap.hesvh.cn/Article/details/griyjdopd.sHtML

[R44] 按修改时间查找
来源：http://m.share.fehbvm.com/Article/details/gygxqxhkp.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fehbvm.com/Article/details/gcxfdrnzw.sHtML

[R45] 批量删除
来源：http://www.share.zdbjq.cn/Article/details/gerdiqhhg.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.zdbjq.cn/Article/details/gjhppzkns.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fehbvm.com/Article/details/ghlgbwjpk.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.zdbjq.cn/Article/details/gestsfubn.sHtML

[R47] sed 单行替换
来源：http://www.share.hesvh.cn/Article/details/gyrvqqeos.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.zdbjq.cn/Article/details/geuvnidrx.sHtML

[R48] awk 取指定列
来源：http://read.share.zdbjq.cn/Article/details/gdcewhdbx.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.zdbjq.cn/Article/details/gqbrtwlyt.sHtML

[R49] awk 带条件
来源：http://read.share.fehbvm.com/Article/details/gnmueobvz.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.fehbvm.com/Article/details/gxrijighj.sHtML

[R50] awk 求和
来源：http://www.m.share.zdbjq.cn/Article/details/gukneuakf.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.hesvh.cn/Article/details/gryanxyyw.sHtML

[R51] 排序去重取前几
来源：http://3g.fehbvm.com/Article/details/gnvigxvki.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.zdbjq.cn/Article/details/gcyepkewx.sHtML

[R52] 统计行数
来源：http://www.share.zdbjq.cn/Article/details/gcjiiiztx.sHtML

wc -l a.txt
来源：http://www.share.zdbjq.cn/Article/details/gwhqguddh.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.fehbvm.com/Article/details/gkryifmui.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fehbvm.com/Article/details/glsgtkckr.sHtML

[R54] 比较两个文件
来源：http://mobile.hesvh.cn/Article/details/gbmzkjioq.sHtML

diff a.txt b.txt
来源：http://www.blog.zdbjq.cn/Article/details/gjokzolcx.sHtML

[R55] 压缩与解压
来源：http://mobile.fehbvm.com/Article/details/gxywswllc.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fehbvm.com/Article/details/gojjzwvsw.sHtML

[R56] 远程拷贝
来源：http://www.share.hesvh.cn/Article/details/gonyokgba.sHtML

scp file user@host:/path/
来源：http://read.share.hesvh.cn/Article/details/gzihxqcmf.sHtML

[R57] 远程执行命令
来源：http://baike.fehbvm.com/Article/details/giassgatt.sHtML

ssh user@host 'uptime'
来源：http://mobile.hesvh.cn/Article/details/gxekxcjrb.sHtML

[R58] 下载文件
来源：http://www.blog.zdbjq.cn/Article/details/gokwqppgv.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fehbvm.com/Article/details/gghvxfyci.sHtML

[R59] 发 POST JSON
来源：http://m.share.zdbjq.cn/Article/details/gyxxkismf.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.hesvh.cn/Article/details/gpbwwkflj.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.hesvh.cn/Article/details/gairhpfrf.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.fehbvm.com/Article/details/govbtbgjd.sHtML

[R61] 磁盘占用
来源：http://www.m.share.hesvh.cn/Article/details/gdazlogeh.sHtML

df -h;  du -sh *
来源：http://mobile.zdbjq.cn/Article/details/goabrhnse.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.zdbjq.cn/Article/details/gcrljstvk.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.zdbjq.cn/Article/details/ggqwgjsoz.sHtML

[R63] 内存与进程
来源：http://m.share.fehbvm.com/Article/details/gbvakfkgt.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fehbvm.com/Article/details/gdsjsybfd.sHtML

[R64] 结束进程
来源：http://m.share.hesvh.cn/Article/details/gsmszflav.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fehbvm.com/Article/details/gruohbqyu.sHtML

[R65] 查看端口占用
来源：http://baike.fehbvm.com/Article/details/gyvprjzyi.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.zdbjq.cn/Article/details/glcqgockp.sHtML

[R66] 定时任务
来源：http://read.share.zdbjq.cn/Article/details/gryaslsht.sHtML

crontab -e;  crontab -l
来源：http://m.share.zdbjq.cn/Article/details/gcozzaysy.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.zdbjq.cn/Article/details/gpatcnmnq.sHtML

openssl rand -hex 16
来源：http://www.blog.zdbjq.cn/Article/details/gokhqfcop.sHtML

[R68] 计算文件校验值
来源：http://baike.hesvh.cn/Article/details/ginqtrtay.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gnhexdxsq.sHtML

[R69] 生成随机密码
来源：http://www.share.zdbjq.cn/Article/details/gzquxlwag.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.zdbjq.cn/Article/details/gfojznssh.sHtML

[R70] 时间戳与互转
来源：http://read.share.hesvh.cn/Article/details/gwmmhdoba.sHtML

date +%s;  date -d @1700000000
来源：http://wap.zdbjq.cn/Article/details/gmrunieos.sHtML

[R71] 日期格式化
来源：http://mobile.hesvh.cn/Article/details/grjhtvnto.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fehbvm.com/Article/details/gdzeezmvd.sHtML

[R72] 等待端口就绪
来源：http://m.share.hesvh.cn/Article/details/ggnsluwhm.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.hesvh.cn/Article/details/gtoiupbvg.sHtML

[R73] 分割大日志
来源：http://www.blog.hesvh.cn/Article/details/gmjzqnhfx.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.hesvh.cn/Article/details/geeyjsoka.sHtML

[R74] 批量重命名
来源：http://read.share.fehbvm.com/Article/details/ghcasnhye.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.fehbvm.com/Article/details/gsfhzaxkc.sHtML

[R75] 导出环境变量
来源：http://www.m.share.hesvh.cn/Article/details/gagouquuq.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.zdbjq.cn/Article/details/gdmxlekyw.sHtML

[R76] 使用临时文件
来源：http://baike.fehbvm.com/Article/details/gukdhfaqp.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fehbvm.com/Article/details/gnoxcfwdn.sHtML

[R77] 读取用户输入
来源：http://m.share.zdbjq.cn/Article/details/gxjvvatyc.sHtML

read -rp "请输入: " ans
来源：http://blog.fehbvm.com/Article/details/gektruuvj.sHtML

[R78] 交互式菜单
来源：http://www.blog.fehbvm.com/Article/details/gkybgwmtt.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.zdbjq.cn/Article/details/gppiyxfqi.sHtML

[R79] 解析命令行选项
来源：http://baike.fehbvm.com/Article/details/ggcgfdosk.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.fehbvm.com/Article/details/gjcxnlnwd.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.zdbjq.cn/Article/details/gpiorjskw.sHtML

time ./run.sh
来源：http://blog.hesvh.cn/Article/details/gecjqbkyv.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/grpmecjjp.sHtML

S. C / C++ 专题
来源：http://mobile.fehbvm.com/Article/details/gcvdcurmu.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gftsgjqqz.sHtML

[S01] C：Hello World
来源：http://read.share.fehbvm.com/Article/details/gxkogrduv.sHtML

#include <stdio.h>
来源：http://www.blog.zdbjq.cn/Article/details/gqmzklnls.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.hesvh.cn/Article/details/gyjsbrpqy.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.zdbjq.cn/Article/details/gpbvqfvmq.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.fehbvm.com/Article/details/gouqloukp.sHtML

[S03] C：读入整数
来源：http://blog.hesvh.cn/Article/details/gilenrmbo.sHtML

int x; scanf("%d", &x);
来源：http://3g.fehbvm.com/Article/details/gbinhrcqc.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fehbvm.com/Article/details/gxtiuglsw.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.zdbjq.cn/Article/details/gbqgoiszk.sHtML

[S05] C：字符串长度
来源：http://mobile.zdbjq.cn/Article/details/gknqqjqmb.sHtML

strlen(s)
来源：http://3g.hesvh.cn/Article/details/ghgmikizy.sHtML

[S06] C：字符串比较
来源：http://www.blog.fehbvm.com/Article/details/gctqrsscb.sHtML

strcmp(a, b) == 0
来源：http://www.blog.zdbjq.cn/Article/details/gduhlprss.sHtML

[S07] C：数组遍历求和
来源：http://blog.fehbvm.com/Article/details/gpazntgni.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.fehbvm.com/Article/details/gilrsummq.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.hesvh.cn/Article/details/gxgqmdsjv.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.zdbjq.cn/Article/details/gxljnyjvh.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.zdbjq.cn/Article/details/gouraioxk.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.hesvh.cn/Article/details/gsmfhxbcb.sHtML

[S10] C：指针与解引用
来源：http://3g.hesvh.cn/Article/details/gzakndtvb.sHtML

int *p = &a;  *p = 5;
来源：http://wap.zdbjq.cn/Article/details/gjyqgthyg.sHtML

[S11] C：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gqwhtlwam.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.hesvh.cn/Article/details/gioamisoh.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.fehbvm.com/Article/details/goqeixuet.sHtML

fclose(f);
来源：http://blog.hesvh.cn/Article/details/gstvjsszw.sHtML

[S12] C：写文件
来源：http://read.share.zdbjq.cn/Article/details/gmepnvzwd.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.hesvh.cn/Article/details/gdvojzrrp.sHtML

[S13] C：宏定义
来源：http://wap.zdbjq.cn/Article/details/gmzjueume.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.hesvh.cn/Article/details/gzxmsigsr.sHtML

[S14] C：枚举
来源：http://www.blog.hesvh.cn/Article/details/gkvmjguve.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.hesvh.cn/Article/details/gsfmgogsd.sHtML

[S15] C：类型转换
来源：http://www.share.zdbjq.cn/Article/details/gwwbjpxml.sHtML

(double) a / b
来源：http://blog.fehbvm.com/Article/details/gmpouzwby.sHtML

[S16] C：位操作置位
来源：http://www.m.share.zdbjq.cn/Article/details/glgmwypfv.sHtML

x |= (1 << 3);
来源：http://www.blog.zdbjq.cn/Article/details/gqvaigihf.sHtML

[S17] C：安全拼接字符串
来源：http://3g.zdbjq.cn/Article/details/gteedcgab.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.zdbjq.cn/Article/details/gvowndbnx.sHtML

[S18] C：命令行参数
来源：http://read.share.hesvh.cn/Article/details/gpvtpdjcp.sHtML

int main(int argc, char **argv)
来源：http://baike.fehbvm.com/Article/details/gxhholgao.sHtML

[S19] C：快速排序
来源：http://baike.fehbvm.com/Article/details/gbngclnfo.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fehbvm.com/Article/details/gbhhlojpk.sHtML

[S20] C：二分查找
来源：http://www.blog.zdbjq.cn/Article/details/gnzfrphfi.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.hesvh.cn/Article/details/gngakcxmt.sHtML

[S21] C：字符类别判断
来源：http://mobile.hesvh.cn/Article/details/gnttdnaem.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.hesvh.cn/Article/details/gzhcpbpqx.sHtML

[S22] C：字符串转数字
来源：http://blog.fehbvm.com/Article/details/gnmragyqr.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.zdbjq.cn/Article/details/gqhuqpxda.sHtML

[S23] C：随机数
来源：http://mobile.fehbvm.com/Article/details/ghhfxtywl.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fehbvm.com/Article/details/gbudszngw.sHtML

[S24] C：获取本地时间
来源：http://m.share.fehbvm.com/Article/details/gigepfiog.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.hesvh.cn/Article/details/gwwwuksdz.sHtML

[S25] C：内存拷贝
来源：http://m.share.fehbvm.com/Article/details/ghhiwgrjt.sHtML

memcpy(dst, src, n);
来源：http://m.share.zdbjq.cn/Article/details/gyebvuakv.sHtML

[S26] C：内存清零
来源：http://blog.hesvh.cn/Article/details/grpzwidkj.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.hesvh.cn/Article/details/gvlduugqp.sHtML

[S27] C：定义常量
来源：http://blog.zdbjq.cn/Article/details/gqzdxxysm.sHtML

const double PI = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gnsidnfta.sHtML

[S28] C：静态变量
来源：http://www.blog.hesvh.cn/Article/details/gtmmitnri.sHtML

static int counter = 0;
来源：http://m.share.zdbjq.cn/Article/details/gnqigqfhw.sHtML

[S29] C：变参函数
来源：http://read.share.hesvh.cn/Article/details/glfpdgwqd.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.hesvh.cn/Article/details/geadneock.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fehbvm.com/Article/details/gfbbohgzg.sHtML

#ifndef X_H
来源：http://www.share.hesvh.cn/Article/details/gpzsfkmdv.sHtML

#define X_H
来源：http://read.share.hesvh.cn/Article/details/gsyfcglnu.sHtML

#endif
来源：http://mobile.fehbvm.com/Article/details/glkeapzrj.sHtML

[S31] C++：Hello World
来源：http://baike.zdbjq.cn/Article/details/ghtzbtpbi.sHtML

#include <iostream>
来源：http://baike.zdbjq.cn/Article/details/gzwgepgoe.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.hesvh.cn/Article/details/giirdaoab.sHtML

[S32] C++：字符串
来源：http://baike.fehbvm.com/Article/details/gcejqtoqm.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fehbvm.com/Article/details/gzqjhgnes.sHtML

[S33] C++：vector 增删
来源：http://mobile.fehbvm.com/Article/details/gltsenivw.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.hesvh.cn/Article/details/gflgykjtq.sHtML

[S34] C++：遍历 vector
来源：http://blog.zdbjq.cn/Article/details/glkaijijs.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.hesvh.cn/Article/details/gmqawreza.sHtML

[S35] C++：map
来源：http://wap.zdbjq.cn/Article/details/gqkfyhstq.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fehbvm.com/Article/details/gpnazgdyd.sHtML

[S36] C++：unordered_map
来源：http://mobile.hesvh.cn/Article/details/gyktpzabm.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gmebdvhfi.sHtML

[S37] C++：set
来源：http://www.blog.hesvh.cn/Article/details/gnsowkirq.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.zdbjq.cn/Article/details/gsnvwyzla.sHtML

[S38] C++：排序
来源：http://blog.zdbjq.cn/Article/details/gwkjqkdjh.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.zdbjq.cn/Article/details/gkgeyserb.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.zdbjq.cn/Article/details/glmdqxpgx.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.zdbjq.cn/Article/details/gexzbqobt.sHtML

[S40] C++：查找元素
来源：http://baike.fehbvm.com/Article/details/gcmhqsfmh.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.hesvh.cn/Article/details/gfjkpcjyl.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.hesvh.cn/Article/details/gwrthtjra.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.fehbvm.com/Article/details/gmdogoujn.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.zdbjq.cn/Article/details/gibxtnaop.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.hesvh.cn/Article/details/gdwkacdxy.sHtML

[S43] C++：智能指针
来源：http://www.m.share.zdbjq.cn/Article/details/gxvfvmpxi.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.hesvh.cn/Article/details/gvipfzobz.sHtML

[S44] C++：引用传参
来源：http://wap.hesvh.cn/Article/details/gpvtryqom.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.hesvh.cn/Article/details/gssisioci.sHtML

[S45] C++：lambda
来源：http://3g.fehbvm.com/Article/details/gfejjlsdv.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.hesvh.cn/Article/details/gnnricleo.sHtML

[S46] C++：函数模板
来源：http://read.share.zdbjq.cn/Article/details/gasetzlss.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fehbvm.com/Article/details/gfihdbxwd.sHtML


<!-- 参考信息 -->