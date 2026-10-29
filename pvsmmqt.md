代发 wailian999

[Q82] 字符长度与字节长度
来源：http://read.share.hesvh.cn/Article/details/gitwbnwlo.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.hesvh.cn/Article/details/gdaqidymp.sHtML

[Q83] 大小写转换
来源：http://baike.zdbjq.cn/Article/details/gujabcrkb.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gsreeqvep.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.fehbvm.com/Article/details/gbhpvjkrn.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gdsdxjlpm.sHtML

[Q85] 数值取整
来源：http://www.m.share.zdbjq.cn/Article/details/glrdvzgiw.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.hesvh.cn/Article/details/gpiumqdwx.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.fehbvm.com/Article/details/gxavpujrb.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.fehbvm.com/Article/details/gtgtacprz.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.zdbjq.cn/Article/details/ghmqxwxiu.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.zdbjq.cn/Article/details/gmpppmpni.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.hesvh.cn/Article/details/gqpexgyzn.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fehbvm.com/Article/details/gpmfkddeh.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.zdbjq.cn/Article/details/ggbhahtir.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.hesvh.cn/Article/details/geekrmdlj.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.zdbjq.cn/Article/details/gitrvfioy.sHtML

[Q90] 生成序号列
来源：http://read.share.hesvh.cn/Article/details/gzuqrpucs.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.hesvh.cn/Article/details/gakcyfwam.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gxrtfefob.sHtML

R. Bash 专题
来源：http://mobile.zdbjq.cn/Article/details/gnccckqmr.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gzdazsxmj.sHtML

[R01] shebang 与严格模式
来源：http://3g.fehbvm.com/Article/details/gnyqyekyx.sHtML

#!/usr/bin/env bash
来源：http://mobile.hesvh.cn/Article/details/ghcnavdnc.sHtML

set -euo pipefail
来源：http://www.blog.zdbjq.cn/Article/details/gxuanervt.sHtML

[R02] 变量赋值与使用
来源：http://read.share.fehbvm.com/Article/details/guynllhij.sHtML

name="Tom"; echo "$name"
来源：http://www.share.fehbvm.com/Article/details/gcqqbghvv.sHtML

[R03] 只读变量
来源：http://www.blog.hesvh.cn/Article/details/gjbatbtfw.sHtML

readonly PI=3.14
来源：http://3g.zdbjq.cn/Article/details/getglhxqj.sHtML

[R04] 位置参数
来源：http://blog.zdbjq.cn/Article/details/genudxesw.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.zdbjq.cn/Article/details/gfjxmhaiz.sHtML

[R05] 参数默认值
来源：http://wap.hesvh.cn/Article/details/gewdurqys.sHtML

name="${1:-default}"
来源：http://blog.hesvh.cn/Article/details/gqyyfkele.sHtML

[R06] 判断命令是否存在
来源：http://read.share.fehbvm.com/Article/details/goyzltfgm.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.zdbjq.cn/Article/details/gahgcudro.sHtML

[R07] if 判断文件
来源：http://3g.fehbvm.com/Article/details/gyhldtozc.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.hesvh.cn/Article/details/gpmzekngi.sHtML

[R08] 数值比较
来源：http://m.share.zdbjq.cn/Article/details/gdyucuknt.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gjoabinee.sHtML

[R09] 字符串比较
来源：http://www.m.share.fehbvm.com/Article/details/gxlfuqzfh.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.hesvh.cn/Article/details/gkrgtreqy.sHtML

[R10] 正则匹配
来源：http://blog.hesvh.cn/Article/details/gtoktstxw.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.hesvh.cn/Article/details/gpfebznjn.sHtML

[R11] case 多分支
来源：http://blog.fehbvm.com/Article/details/gwmkgckbq.sHtML

case "$1" in
来源：http://www.blog.hesvh.cn/Article/details/gobtlhqas.sHtML

start) echo "启动" ;;
来源：http://blog.hesvh.cn/Article/details/givxmrrzp.sHtML

stop)  echo "停止" ;;
来源：http://mobile.zdbjq.cn/Article/details/gxfhkehpf.sHtML

*)     echo "未知命令" ;;
来源：http://wap.hesvh.cn/Article/details/gpksgghlq.sHtML

esac
来源：http://3g.fehbvm.com/Article/details/gifqhlkom.sHtML

[R12] for 遍历文件
来源：http://www.m.share.zdbjq.cn/Article/details/gqebrfxtl.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.hesvh.cn/Article/details/gkxiblmmk.sHtML

[R13] for 计数循环
来源：http://m.share.zdbjq.cn/Article/details/grsajjolu.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.hesvh.cn/Article/details/govaqdqba.sHtML

[R14] C 风格 for
来源：http://www.m.share.zdbjq.cn/Article/details/gcgkwmstx.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gzvhqwsnc.sHtML

[R15] while 逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gppewpcrv.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.hesvh.cn/Article/details/glucnhkea.sHtML

[R16] until 等待条件
来源：http://www.blog.hesvh.cn/Article/details/gapqfhqru.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.fehbvm.com/Article/details/gnqurdcrn.sHtML

[R17] 数组定义与取值
来源：http://www.blog.fehbvm.com/Article/details/gkkvgraxe.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.zdbjq.cn/Article/details/gyfjauikq.sHtML

[R18] 遍历数组
来源：http://baike.zdbjq.cn/Article/details/gahzkfvgj.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.hesvh.cn/Article/details/gricxvqyn.sHtML

[R19] 数组长度
来源：http://wap.hesvh.cn/Article/details/gfeysakus.sHtML

echo "${#arr[@]}"
来源：http://baike.fehbvm.com/Article/details/gkysxusla.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.hesvh.cn/Article/details/gyxvkqmck.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.zdbjq.cn/Article/details/gdrupdhnu.sHtML

[R21] 字符串长度
来源：http://baike.hesvh.cn/Article/details/gklzrdmhm.sHtML

echo "${#s}"
来源：http://www.blog.fehbvm.com/Article/details/gdajesjrv.sHtML

[R22] 截取子串
来源：http://www.share.zdbjq.cn/Article/details/gttmhaddg.sHtML

echo "${s:0:5}"
来源：http://www.blog.hesvh.cn/Article/details/gqtfcdsoh.sHtML

[R23] 字符串替换
来源：http://3g.fehbvm.com/Article/details/goeggrbel.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.zdbjq.cn/Article/details/gigfkrmxp.sHtML

[R24] 大小写转换
来源：http://baike.zdbjq.cn/Article/details/gtpmrzofe.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.hesvh.cn/Article/details/gajayjxes.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.fehbvm.com/Article/details/gpruewsuy.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.zdbjq.cn/Article/details/gzcbtqiex.sHtML

[R26] 命令替换
来源：http://mobile.zdbjq.cn/Article/details/gmzjkrvce.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.zdbjq.cn/Article/details/ggmzdzybd.sHtML

[R27] 算术展开
来源：http://blog.fehbvm.com/Article/details/gxzohbwrr.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.fehbvm.com/Article/details/gcfkrqwlo.sHtML

[R28] 浮点运算
来源：http://mobile.zdbjq.cn/Article/details/gofkiqhwa.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.hesvh.cn/Article/details/gvnfkesrx.sHtML

[R29] 定义函数
来源：http://blog.hesvh.cn/Article/details/gjjxosusn.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.zdbjq.cn/Article/details/glkfrftvn.sHtML

[R30] 函数返回状态码
来源：http://3g.fehbvm.com/Article/details/gyfmmoekl.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.zdbjq.cn/Article/details/gifdkhvfp.sHtML

[R31] 局部变量
来源：http://read.share.hesvh.cn/Article/details/ggiymzqlf.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.hesvh.cn/Article/details/gslwhzokm.sHtML

[R32] 参数个数校验
来源：http://mobile.hesvh.cn/Article/details/gowdhkyyc.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.zdbjq.cn/Article/details/gcuklldah.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.zdbjq.cn/Article/details/gfpbrctuo.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.fehbvm.com/Article/details/gtyyyqxve.sHtML

[R34] 退出时清理
来源：http://www.m.share.hesvh.cn/Article/details/gwbhnoyez.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.hesvh.cn/Article/details/ghxzeqlgp.sHtML

[R35] 后台执行并等待
来源：http://www.blog.hesvh.cn/Article/details/gwbavivbk.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.hesvh.cn/Article/details/gzofguipb.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.hesvh.cn/Article/details/gmihmmuhx.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.zdbjq.cn/Article/details/gseqciwxd.sHtML

[R37] 把输出赋给变量
来源：http://blog.hesvh.cn/Article/details/gbybwdsjs.sHtML

files=$(ls -1)
来源：http://read.share.zdbjq.cn/Article/details/gwdlhfvae.sHtML

[R38] 管道串联
来源：http://3g.fehbvm.com/Article/details/ggqhiqqub.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.hesvh.cn/Article/details/giailjkkp.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.hesvh.cn/Article/details/gfjzozrba.sHtML

cmd > out.log 2>&1
来源：http://www.share.fehbvm.com/Article/details/gtqdcatjj.sHtML

[R40] 追加写日志
来源：http://www.share.fehbvm.com/Article/details/gjyjrtctu.sHtML

echo "log" >> out.log
来源：http://read.share.hesvh.cn/Article/details/grzzfwdqt.sHtML

[R41] 丢弃输出
来源：http://3g.zdbjq.cn/Article/details/godxdedam.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.fehbvm.com/Article/details/gtcrjevkh.sHtML

[R42] 输入重定向
来源：http://3g.hesvh.cn/Article/details/gequzwrjo.sHtML

wc -l < a.txt
来源：http://wap.hesvh.cn/Article/details/ghkjiaxto.sHtML

[R43] 按名字查找文件
来源：http://m.share.hesvh.cn/Article/details/gjjddgzey.sHtML

find . -name "*.log" -type f
来源：http://blog.fehbvm.com/Article/details/gqqutcgsm.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fehbvm.com/Article/details/gejmsiqrk.sHtML

find . -mtime -7 -type f
来源：http://wap.fehbvm.com/Article/details/gyvauauyf.sHtML

[R45] 批量删除
来源：http://mobile.zdbjq.cn/Article/details/gsrifkpii.sHtML

find . -name "*.tmp" -delete
来源：http://wap.hesvh.cn/Article/details/gltljgzid.sHtML

[R46] 递归替换文件内容
来源：http://3g.fehbvm.com/Article/details/gtxfmqscr.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.hesvh.cn/Article/details/gkdxfrhrv.sHtML

[R47] sed 单行替换
来源：http://www.share.hesvh.cn/Article/details/gicilmbph.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.zdbjq.cn/Article/details/gflwdeidw.sHtML

[R48] awk 取指定列
来源：http://m.share.fehbvm.com/Article/details/gwmttsdhd.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.hesvh.cn/Article/details/gmbtdsbyo.sHtML

[R49] awk 带条件
来源：http://mobile.hesvh.cn/Article/details/gfxetjmqj.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.hesvh.cn/Article/details/gwmlrhlzv.sHtML

[R50] awk 求和
来源：http://www.m.share.fehbvm.com/Article/details/gqpdgrydk.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/grsedtonj.sHtML

[R51] 排序去重取前几
来源：http://www.share.hesvh.cn/Article/details/ghdrfubqn.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.fehbvm.com/Article/details/gwajlrrwl.sHtML

[R52] 统计行数
来源：http://3g.fehbvm.com/Article/details/gcdavrano.sHtML

wc -l a.txt
来源：http://wap.fehbvm.com/Article/details/gvbxrtmqq.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.zdbjq.cn/Article/details/guhfhmgea.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.fehbvm.com/Article/details/gfkidopnv.sHtML

[R54] 比较两个文件
来源：http://baike.zdbjq.cn/Article/details/gngaupjfk.sHtML

diff a.txt b.txt
来源：http://wap.hesvh.cn/Article/details/gosbncwxm.sHtML

[R55] 压缩与解压
来源：http://baike.hesvh.cn/Article/details/gkundscje.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.zdbjq.cn/Article/details/gfazszogf.sHtML

[R56] 远程拷贝
来源：http://wap.zdbjq.cn/Article/details/gbytlwqqg.sHtML

scp file user@host:/path/
来源：http://3g.zdbjq.cn/Article/details/glhmsaomr.sHtML

[R57] 远程执行命令
来源：http://wap.hesvh.cn/Article/details/gyegsqqrr.sHtML

ssh user@host 'uptime'
来源：http://www.share.fehbvm.com/Article/details/gvgszagtm.sHtML

[R58] 下载文件
来源：http://wap.zdbjq.cn/Article/details/goujiwire.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.fehbvm.com/Article/details/gkdjtsspu.sHtML

[R59] 发 POST JSON
来源：http://blog.hesvh.cn/Article/details/gipklackr.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.hesvh.cn/Article/details/gsrsxyvwt.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.zdbjq.cn/Article/details/gliqurply.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.zdbjq.cn/Article/details/gpmtzgbgr.sHtML

[R61] 磁盘占用
来源：http://read.share.zdbjq.cn/Article/details/gjihhbuja.sHtML

df -h;  du -sh *
来源：http://baike.hesvh.cn/Article/details/gyyblqxtz.sHtML

[R62] 找最占空间的文件
来源：http://baike.zdbjq.cn/Article/details/gcuovlkox.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.fehbvm.com/Article/details/gtwtzoxfl.sHtML

[R63] 内存与进程
来源：http://m.share.hesvh.cn/Article/details/gptlyfmgq.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fehbvm.com/Article/details/gtajqouak.sHtML

[R64] 结束进程
来源：http://blog.hesvh.cn/Article/details/gvyjouaed.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.zdbjq.cn/Article/details/gzennrvvf.sHtML

[R65] 查看端口占用
来源：http://m.share.zdbjq.cn/Article/details/gqtdpdvqm.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.fehbvm.com/Article/details/gjugbnrmq.sHtML

[R66] 定时任务
来源：http://blog.zdbjq.cn/Article/details/gtsrbvsbv.sHtML

crontab -e;  crontab -l
来源：http://wap.hesvh.cn/Article/details/gytecxtoz.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.hesvh.cn/Article/details/gwocgbhif.sHtML

openssl rand -hex 16
来源：http://baike.zdbjq.cn/Article/details/gayttkouo.sHtML

[R68] 计算文件校验值
来源：http://read.share.hesvh.cn/Article/details/glqdasnjv.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.zdbjq.cn/Article/details/gwjkruaol.sHtML

[R69] 生成随机密码
来源：http://read.share.hesvh.cn/Article/details/gvcyihpfe.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fehbvm.com/Article/details/ggmpbhcui.sHtML

[R70] 时间戳与互转
来源：http://mobile.fehbvm.com/Article/details/gujwgvnbd.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.zdbjq.cn/Article/details/gegcxqnve.sHtML

[R71] 日期格式化
来源：http://3g.zdbjq.cn/Article/details/guxhutmrh.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.hesvh.cn/Article/details/gkjlejruc.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.hesvh.cn/Article/details/gmhtpugwk.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.zdbjq.cn/Article/details/gpvnsnbdx.sHtML

[R73] 分割大日志
来源：http://www.blog.hesvh.cn/Article/details/gyqwehcrv.sHtML

split -l 1000 big.log part_
来源：http://baike.hesvh.cn/Article/details/gpytrkpad.sHtML

[R74] 批量重命名
来源：http://wap.fehbvm.com/Article/details/ghgismyev.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.zdbjq.cn/Article/details/gjhkljcbw.sHtML

[R75] 导出环境变量
来源：http://m.share.hesvh.cn/Article/details/gpfhvyrdz.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.fehbvm.com/Article/details/glmmdytzn.sHtML

[R76] 使用临时文件
来源：http://m.share.fehbvm.com/Article/details/gqpzeybuk.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.hesvh.cn/Article/details/gdeluzmto.sHtML

[R77] 读取用户输入
来源：http://baike.fehbvm.com/Article/details/grwjcpmuo.sHtML

read -rp "请输入: " ans
来源：http://blog.fehbvm.com/Article/details/gnrfhxemv.sHtML

[R78] 交互式菜单
来源：http://mobile.hesvh.cn/Article/details/gtbttnmzp.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.hesvh.cn/Article/details/gkslahlxr.sHtML

[R79] 解析命令行选项
来源：http://blog.zdbjq.cn/Article/details/gnnneuwse.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.fehbvm.com/Article/details/gdzixrdln.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.fehbvm.com/Article/details/gbytguhay.sHtML

time ./run.sh
来源：http://3g.fehbvm.com/Article/details/gbenourvn.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gbmbpemph.sHtML

S. C / C++ 专题
来源：http://read.share.fehbvm.com/Article/details/goaaecgfz.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gwylfbpyp.sHtML

[S01] C：Hello World
来源：http://m.share.zdbjq.cn/Article/details/goiroqzkm.sHtML

#include <stdio.h>
来源：http://mobile.zdbjq.cn/Article/details/gbzzzcqlk.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.zdbjq.cn/Article/details/gekbjzmoe.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fehbvm.com/Article/details/gwwgaodmr.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.fehbvm.com/Article/details/gtwthbsak.sHtML

[S03] C：读入整数
来源：http://wap.fehbvm.com/Article/details/gpcosglzs.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.fehbvm.com/Article/details/gckmafqdn.sHtML

[S04] C：字符串复制
来源：http://m.share.hesvh.cn/Article/details/gqztjaguf.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.hesvh.cn/Article/details/gotesaqbs.sHtML

[S05] C：字符串长度
来源：http://m.share.fehbvm.com/Article/details/gvwvonqrn.sHtML

strlen(s)
来源：http://mobile.fehbvm.com/Article/details/gxuhuzkck.sHtML

[S06] C：字符串比较
来源：http://mobile.zdbjq.cn/Article/details/gqybevjun.sHtML

strcmp(a, b) == 0
来源：http://baike.fehbvm.com/Article/details/gmmtiiltq.sHtML

[S07] C：数组遍历求和
来源：http://www.share.fehbvm.com/Article/details/gllribboc.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fehbvm.com/Article/details/gxvyipber.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.hesvh.cn/Article/details/gfcedpymh.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.zdbjq.cn/Article/details/gocekrzuk.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fehbvm.com/Article/details/gxlsjjnmc.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.zdbjq.cn/Article/details/gxzsdbard.sHtML

[S10] C：指针与解引用
来源：http://m.share.hesvh.cn/Article/details/gemiuapwn.sHtML

int *p = &a;  *p = 5;
来源：http://baike.hesvh.cn/Article/details/gnqhwugam.sHtML

[S11] C：逐行读文件
来源：http://blog.fehbvm.com/Article/details/gwuvsxnak.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.fehbvm.com/Article/details/gpmruafjb.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.hesvh.cn/Article/details/glfbneltp.sHtML

fclose(f);
来源：http://read.share.zdbjq.cn/Article/details/gvcuoazwv.sHtML

[S12] C：写文件
来源：http://baike.hesvh.cn/Article/details/grprzcalj.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fehbvm.com/Article/details/gcvhnnrha.sHtML

[S13] C：宏定义
来源：http://blog.hesvh.cn/Article/details/gcwvnhwzx.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.hesvh.cn/Article/details/gykdlnjlt.sHtML

[S14] C：枚举
来源：http://www.share.fehbvm.com/Article/details/gcrqmhqvc.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.hesvh.cn/Article/details/gbxpdfqyo.sHtML

[S15] C：类型转换
来源：http://www.blog.zdbjq.cn/Article/details/gqwxivjvy.sHtML

(double) a / b
来源：http://www.m.share.fehbvm.com/Article/details/gqunkvghz.sHtML

[S16] C：位操作置位
来源：http://m.share.fehbvm.com/Article/details/gyijtpsxi.sHtML

x |= (1 << 3);
来源：http://m.share.hesvh.cn/Article/details/gvkajrbtw.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.zdbjq.cn/Article/details/grcuogwpu.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.zdbjq.cn/Article/details/gzlstcjzv.sHtML

[S18] C：命令行参数
来源：http://www.m.share.zdbjq.cn/Article/details/ggjdgyatv.sHtML

int main(int argc, char **argv)
来源：http://read.share.hesvh.cn/Article/details/gknwwdesv.sHtML

[S19] C：快速排序
来源：http://www.share.hesvh.cn/Article/details/ghbeqbdps.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fehbvm.com/Article/details/gmfnlscjg.sHtML

[S20] C：二分查找
来源：http://3g.hesvh.cn/Article/details/gtdbfhilh.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fehbvm.com/Article/details/giudbyeuk.sHtML

[S21] C：字符类别判断
来源：http://www.share.hesvh.cn/Article/details/grtwnqzrc.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.zdbjq.cn/Article/details/gtugqwktv.sHtML

[S22] C：字符串转数字
来源：http://wap.zdbjq.cn/Article/details/gxwffftaq.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.hesvh.cn/Article/details/gtizclvwl.sHtML

[S23] C：随机数
来源：http://baike.hesvh.cn/Article/details/gvqsaxsxz.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.fehbvm.com/Article/details/gasyncxdc.sHtML

[S24] C：获取本地时间
来源：http://blog.fehbvm.com/Article/details/ghhxcqylb.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fehbvm.com/Article/details/gzqwnwgqy.sHtML

[S25] C：内存拷贝
来源：http://m.share.hesvh.cn/Article/details/grdoskyhe.sHtML

memcpy(dst, src, n);
来源：http://3g.hesvh.cn/Article/details/gmuslsgpo.sHtML

[S26] C：内存清零
来源：http://www.m.share.fehbvm.com/Article/details/gznhizwds.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.hesvh.cn/Article/details/gmfqzkfze.sHtML

[S27] C：定义常量
来源：http://www.m.share.fehbvm.com/Article/details/gqarcyrww.sHtML

const double PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gpshutcvk.sHtML

[S28] C：静态变量
来源：http://www.m.share.fehbvm.com/Article/details/gjcpgmqgw.sHtML

static int counter = 0;
来源：http://read.share.fehbvm.com/Article/details/ggfrdqlly.sHtML

[S29] C：变参函数
来源：http://baike.hesvh.cn/Article/details/gtnyuyjkb.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fehbvm.com/Article/details/gjgjkmftb.sHtML

[S30] C：头文件保护
来源：http://mobile.fehbvm.com/Article/details/gooxfmyqq.sHtML

#ifndef X_H
来源：http://www.share.fehbvm.com/Article/details/gzayrewpq.sHtML

#define X_H
来源：http://mobile.fehbvm.com/Article/details/gxzryjtxt.sHtML

#endif
来源：http://www.share.fehbvm.com/Article/details/grsqexpnw.sHtML

[S31] C++：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gskbuzfmw.sHtML

#include <iostream>
来源：http://mobile.fehbvm.com/Article/details/globgsqcw.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.hesvh.cn/Article/details/glnotqjxm.sHtML

[S32] C++：字符串
来源：http://www.share.fehbvm.com/Article/details/gqudagaiy.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fehbvm.com/Article/details/gfwxpfyrv.sHtML

[S33] C++：vector 增删
来源：http://m.share.hesvh.cn/Article/details/gksjpdway.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gzqcjoykd.sHtML

[S34] C++：遍历 vector
来源：http://blog.hesvh.cn/Article/details/gyzilvjzc.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.hesvh.cn/Article/details/gskodtfzv.sHtML

[S35] C++：map
来源：http://baike.zdbjq.cn/Article/details/gjioziccd.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/ghbcmbeyx.sHtML

[S36] C++：unordered_map
来源：http://mobile.fehbvm.com/Article/details/gqndsxytj.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/grurawbzf.sHtML

[S37] C++：set
来源：http://mobile.fehbvm.com/Article/details/goitzlmhj.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.zdbjq.cn/Article/details/ghsmjxdwx.sHtML

[S38] C++：排序
来源：http://blog.zdbjq.cn/Article/details/geeajkqff.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.hesvh.cn/Article/details/gopfxwdzo.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.zdbjq.cn/Article/details/gjlypysdr.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.zdbjq.cn/Article/details/gqcdrenfq.sHtML

[S40] C++：查找元素
来源：http://www.share.fehbvm.com/Article/details/ghmhentes.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.fehbvm.com/Article/details/gndglzqpi.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.fehbvm.com/Article/details/goanadhnb.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.zdbjq.cn/Article/details/grnidmbrw.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.zdbjq.cn/Article/details/gmowjityr.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.fehbvm.com/Article/details/gwkuhsjqi.sHtML

[S43] C++：智能指针
来源：http://baike.fehbvm.com/Article/details/gxakrnylu.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.hesvh.cn/Article/details/gexvncgte.sHtML

[S44] C++：引用传参
来源：http://baike.fehbvm.com/Article/details/gzknbubxz.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.zdbjq.cn/Article/details/glubgyggf.sHtML

[S45] C++：lambda
来源：http://baike.hesvh.cn/Article/details/gpmvskomp.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.fehbvm.com/Article/details/gcptzvtxa.sHtML

[S46] C++：函数模板
来源：http://wap.zdbjq.cn/Article/details/gwbgtinsb.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.hesvh.cn/Article/details/gymzemrrl.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.fehbvm.com/Article/details/gspgizhub.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.fehbvm.com/Article/details/ggkxykltf.sHtML

[S48] C++：逐行读文件
来源：http://baike.hesvh.cn/Article/details/ghmitjeak.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fehbvm.com/Article/details/gruopfgev.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.hesvh.cn/Article/details/gzzkcimca.sHtML

[S49] C++：写文件
来源：http://www.share.fehbvm.com/Article/details/gfpiksjsr.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.zdbjq.cn/Article/details/ggrxxtnsb.sHtML

[S50] C++：格式化数字
来源：http://wap.fehbvm.com/Article/details/gdaaovvxe.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gheimrpgm.sHtML

[S51] C++：显式类型转换
来源：http://3g.zdbjq.cn/Article/details/gwzcwsinl.sHtML

static_cast<double>(a) / b
来源：http://wap.hesvh.cn/Article/details/gigpajtvf.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.hesvh.cn/Article/details/gffuceuab.sHtML


<!-- 参考信息 -->