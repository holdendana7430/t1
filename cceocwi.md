代发 wailian999

[Q88] 行转列（条件聚合）
来源：http://wap.fanxiaobao.xyz/Article/details/gzersliol.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.fanxiaobao.xyz/Article/details/gpxsyhvzz.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/ggsovrwzt.sHtML

[Q89] 判断表是否存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gkpditwno.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.fanxiaobao.xyz/Article/details/gnstcpitv.sHtML

[Q90] 生成序号列
来源：http://blog.fanxiaobao.xyz/Article/details/grefaisox.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.fanxiaobao.xyz/Article/details/gaexhcvpo.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gzbqygtwm.sHtML

R. Bash 专题
来源：http://blog.fanxiaobao.xyz/Article/details/gkjliiwwr.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gvogregyf.sHtML

[R01] shebang 与严格模式
来源：http://baike.fanxiaobao.xyz/Article/details/gchdowdta.sHtML

#!/usr/bin/env bash
来源：http://mobile.fanxiaobao.xyz/Article/details/gytyttbfn.sHtML

set -euo pipefail
来源：http://www.share.fanxiaobao.xyz/Article/details/gxhqzcfco.sHtML

[R02] 变量赋值与使用
来源：http://mobile.fanxiaobao.xyz/Article/details/ghvgfnata.sHtML

name="Tom"; echo "$name"
来源：http://baike.fanxiaobao.xyz/Article/details/ggzwuflto.sHtML

[R03] 只读变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwxidhspw.sHtML

readonly PI=3.14
来源：http://www.share.fanxiaobao.xyz/Article/details/gbupbjsxr.sHtML

[R04] 位置参数
来源：http://3g.fanxiaobao.xyz/Article/details/gchonshmj.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.fanxiaobao.xyz/Article/details/gkowddmac.sHtML

[R05] 参数默认值
来源：http://mobile.fanxiaobao.xyz/Article/details/ggxxfzuno.sHtML

name="${1:-default}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gadtusjjl.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbhcelpwa.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcijfbmpo.sHtML

[R07] if 判断文件
来源：http://3g.fanxiaobao.xyz/Article/details/gkybvstmh.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/glugwyxhi.sHtML

[R08] 数值比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gpfsmzuda.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gxfylkbuy.sHtML

[R09] 字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmtknzlxo.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gykgkynnx.sHtML

[R10] 正则匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gctyeecjn.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gvldonzhb.sHtML

[R11] case 多分支
来源：http://www.blog.fanxiaobao.xyz/Article/details/girsfqjgn.sHtML

case "$1" in
来源：http://blog.fanxiaobao.xyz/Article/details/gzhchbdus.sHtML

start) echo "启动" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gilfruass.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqgdkujnk.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/gxwybucvn.sHtML

esac
来源：http://blog.fanxiaobao.xyz/Article/details/gpdqkhkmt.sHtML

[R12] for 遍历文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnexafvze.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gmeusfagq.sHtML

[R13] for 计数循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grhacvbqb.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gkfewddvm.sHtML

[R14] C 风格 for
来源：http://baike.fanxiaobao.xyz/Article/details/gtnamzmdr.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gpiynqzqj.sHtML

[R15] while 逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gernslcmc.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.fanxiaobao.xyz/Article/details/guhucnffe.sHtML

[R16] until 等待条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gsaiokqfp.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/ggwcmhnsn.sHtML

[R17] 数组定义与取值
来源：http://wap.fanxiaobao.xyz/Article/details/giqumnmjk.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gkrhswtkq.sHtML

[R18] 遍历数组
来源：http://www.share.fanxiaobao.xyz/Article/details/ghuklemvz.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.fanxiaobao.xyz/Article/details/goccomrlr.sHtML

[R19] 数组长度
来源：http://3g.fanxiaobao.xyz/Article/details/gcevtgyzg.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpfdqdcyo.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggulzeyxk.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gdqnfzqeh.sHtML

[R21] 字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gedghxfns.sHtML

echo "${#s}"
来源：http://3g.fanxiaobao.xyz/Article/details/gljdvoixs.sHtML

[R22] 截取子串
来源：http://baike.fanxiaobao.xyz/Article/details/gvtqddwst.sHtML

echo "${s:0:5}"
来源：http://read.share.fanxiaobao.xyz/Article/details/grnxvteqj.sHtML

[R23] 字符串替换
来源：http://3g.fanxiaobao.xyz/Article/details/gptagrzvs.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gwvfhkgny.sHtML

[R24] 大小写转换
来源：http://baike.fanxiaobao.xyz/Article/details/gaymdyoaf.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gcrsojimt.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fanxiaobao.xyz/Article/details/gytvywstf.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gnkrxuepf.sHtML

[R26] 命令替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gxvxvdhey.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcpgyobwi.sHtML

[R27] 算术展开
来源：http://www.share.fanxiaobao.xyz/Article/details/gcshkicuh.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fanxiaobao.xyz/Article/details/gqlapycrf.sHtML

[R28] 浮点运算
来源：http://wap.fanxiaobao.xyz/Article/details/gzpbddptt.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.fanxiaobao.xyz/Article/details/gjrjzzhhy.sHtML

[R29] 定义函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gqvoguhcp.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fanxiaobao.xyz/Article/details/glzsymgsn.sHtML

[R30] 函数返回状态码
来源：http://wap.fanxiaobao.xyz/Article/details/gjumqonrs.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.fanxiaobao.xyz/Article/details/gsvokswlb.sHtML

[R31] 局部变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gntkmzrgz.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gxmkkadws.sHtML

[R32] 参数个数校验
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwnyaatdj.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/glpwbjjgi.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fanxiaobao.xyz/Article/details/gxesmbudo.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.fanxiaobao.xyz/Article/details/grqeiftob.sHtML

[R34] 退出时清理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqpckjole.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/gzbwhtqgh.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goelidmrw.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.fanxiaobao.xyz/Article/details/gidamlxer.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gwsidooxy.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.fanxiaobao.xyz/Article/details/gmdjektci.sHtML

[R37] 把输出赋给变量
来源：http://wap.fanxiaobao.xyz/Article/details/gnixysyhg.sHtML

files=$(ls -1)
来源：http://3g.fanxiaobao.xyz/Article/details/gybllmoox.sHtML

[R38] 管道串联
来源：http://m.share.fanxiaobao.xyz/Article/details/gpzuieria.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.fanxiaobao.xyz/Article/details/gkotqtksd.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.fanxiaobao.xyz/Article/details/gzjilqlvs.sHtML

cmd > out.log 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/gwgmdijgm.sHtML

[R40] 追加写日志
来源：http://wap.fanxiaobao.xyz/Article/details/gkeuwpaon.sHtML

echo "log" >> out.log
来源：http://read.share.fanxiaobao.xyz/Article/details/gfrlfikec.sHtML

[R41] 丢弃输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gndqyugzk.sHtML

cmd >/dev/null 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gcaaxvslg.sHtML

[R42] 输入重定向
来源：http://www.blog.fanxiaobao.xyz/Article/details/gctycsphf.sHtML

wc -l < a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gfktrhoov.sHtML

[R43] 按名字查找文件
来源：http://m.share.fanxiaobao.xyz/Article/details/ggykwwmkj.sHtML

find . -name "*.log" -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjqdbytqk.sHtML

[R44] 按修改时间查找
来源：http://3g.fanxiaobao.xyz/Article/details/gsdrwylpg.sHtML

find . -mtime -7 -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/gcgcccinb.sHtML

[R45] 批量删除
来源：http://read.share.fanxiaobao.xyz/Article/details/gxvdcqzrx.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.fanxiaobao.xyz/Article/details/ggzzwyppb.sHtML

[R46] 递归替换文件内容
来源：http://www.share.fanxiaobao.xyz/Article/details/gvwfwpddq.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjufwhtgy.sHtML

[R47] sed 单行替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gpinszthd.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gndokvsuq.sHtML

[R48] awk 取指定列
来源：http://read.share.fanxiaobao.xyz/Article/details/gtgppfymp.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghryxtwii.sHtML

[R49] awk 带条件
来源：http://wap.fanxiaobao.xyz/Article/details/gcplkosgr.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fanxiaobao.xyz/Article/details/gqoptdxjr.sHtML

[R50] awk 求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gvvshydud.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gnavccsxf.sHtML

[R51] 排序去重取前几
来源：http://m.share.fanxiaobao.xyz/Article/details/gsjqtyqeq.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fanxiaobao.xyz/Article/details/gwmhrizbd.sHtML

[R52] 统计行数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guohpequk.sHtML

wc -l a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gnxjhevew.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.fanxiaobao.xyz/Article/details/gzyepvyxi.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.fanxiaobao.xyz/Article/details/graxgzjop.sHtML

[R54] 比较两个文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gthwtqkut.sHtML

diff a.txt b.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gnxivgoro.sHtML

[R55] 压缩与解压
来源：http://baike.fanxiaobao.xyz/Article/details/gtttwwfkq.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.fanxiaobao.xyz/Article/details/gyyavhtwk.sHtML

[R56] 远程拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/gvwfgdodc.sHtML

scp file user@host:/path/
来源：http://www.blog.fanxiaobao.xyz/Article/details/giuzxpovj.sHtML

[R57] 远程执行命令
来源：http://blog.fanxiaobao.xyz/Article/details/gwjaxljqr.sHtML

ssh user@host 'uptime'
来源：http://read.share.fanxiaobao.xyz/Article/details/gczukqjxw.sHtML

[R58] 下载文件
来源：http://wap.fanxiaobao.xyz/Article/details/gdcgdkxsd.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.fanxiaobao.xyz/Article/details/glhecdowu.sHtML

[R59] 发 POST JSON
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzgbeugml.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.fanxiaobao.xyz/Article/details/ghdxqpysd.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fanxiaobao.xyz/Article/details/grsypdvte.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.fanxiaobao.xyz/Article/details/gfwmmuqjj.sHtML

[R61] 磁盘占用
来源：http://mobile.fanxiaobao.xyz/Article/details/gmjbsvzdu.sHtML

df -h;  du -sh *
来源：http://www.share.fanxiaobao.xyz/Article/details/gyycxudyp.sHtML

[R62] 找最占空间的文件
来源：http://wap.fanxiaobao.xyz/Article/details/gtgedjbeh.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.fanxiaobao.xyz/Article/details/ggqvtyoll.sHtML

[R63] 内存与进程
来源：http://www.share.fanxiaobao.xyz/Article/details/gtgbdduls.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.fanxiaobao.xyz/Article/details/gmskeobsp.sHtML

[R64] 结束进程
来源：http://read.share.fanxiaobao.xyz/Article/details/geqwnzolx.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fanxiaobao.xyz/Article/details/goolmzrfs.sHtML

[R65] 查看端口占用
来源：http://read.share.fanxiaobao.xyz/Article/details/ghweamolr.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fanxiaobao.xyz/Article/details/ghqypwhsn.sHtML

[R66] 定时任务
来源：http://mobile.fanxiaobao.xyz/Article/details/grcmvbpwf.sHtML

crontab -e;  crontab -l
来源：http://www.share.fanxiaobao.xyz/Article/details/gzfjohwsp.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fanxiaobao.xyz/Article/details/gjslaczle.sHtML

openssl rand -hex 16
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcskxxpxs.sHtML

[R68] 计算文件校验值
来源：http://mobile.fanxiaobao.xyz/Article/details/ggmdhtgow.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfechwrwh.sHtML

[R69] 生成随机密码
来源：http://mobile.fanxiaobao.xyz/Article/details/gzdakwkmi.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gocegyueq.sHtML

[R70] 时间戳与互转
来源：http://mobile.fanxiaobao.xyz/Article/details/ggykosgub.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.fanxiaobao.xyz/Article/details/gbymqgpjf.sHtML

[R71] 日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaerhvien.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gozdnjfha.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glxrezgem.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/gintllhgo.sHtML

[R73] 分割大日志
来源：http://blog.fanxiaobao.xyz/Article/details/gimcbwqca.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gohlzhnkf.sHtML

[R74] 批量重命名
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjtkxvexg.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gifdwvjvd.sHtML

[R75] 导出环境变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkelycuto.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.fanxiaobao.xyz/Article/details/gilzabfvy.sHtML

[R76] 使用临时文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gcxpudwcg.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/gdjmpsygn.sHtML

[R77] 读取用户输入
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqjvkuqny.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggwfifmwy.sHtML

[R78] 交互式菜单
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbxhhadnx.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fanxiaobao.xyz/Article/details/ggczzaqhp.sHtML

[R79] 解析命令行选项
来源：http://read.share.fanxiaobao.xyz/Article/details/gbompkzar.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.fanxiaobao.xyz/Article/details/gewbjevsb.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.fanxiaobao.xyz/Article/details/gmuuhlsvi.sHtML

time ./run.sh
来源：http://baike.fanxiaobao.xyz/Article/details/gkipoezmj.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gksynzvzb.sHtML

S. C / C++ 专题
来源：http://read.share.fanxiaobao.xyz/Article/details/gezapvucm.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghdkgydlb.sHtML

[S01] C：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggfkqcimh.sHtML

#include <stdio.h>
来源：http://blog.fanxiaobao.xyz/Article/details/gxwqihpnk.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gchangtrk.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gikxrtfba.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtshfzspp.sHtML

[S03] C：读入整数
来源：http://wap.fanxiaobao.xyz/Article/details/gsdrtbbiz.sHtML

int x; scanf("%d", &x);
来源：http://blog.fanxiaobao.xyz/Article/details/gyymamuip.sHtML

[S04] C：字符串复制
来源：http://3g.fanxiaobao.xyz/Article/details/geoosprpv.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.fanxiaobao.xyz/Article/details/gpekqshfc.sHtML

[S05] C：字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/ghqzynwoe.sHtML

strlen(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gmxyjevle.sHtML

[S06] C：字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/gkxbvummq.sHtML

strcmp(a, b) == 0
来源：http://www.share.fanxiaobao.xyz/Article/details/gzvaegpgz.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fanxiaobao.xyz/Article/details/ghlmkayrt.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjusrjbvv.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.fanxiaobao.xyz/Article/details/gmxgaboup.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.fanxiaobao.xyz/Article/details/gtkdwcatl.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fanxiaobao.xyz/Article/details/gkmvldclb.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.fanxiaobao.xyz/Article/details/gpubyeylp.sHtML

[S10] C：指针与解引用
来源：http://m.share.fanxiaobao.xyz/Article/details/geubynafw.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fanxiaobao.xyz/Article/details/ggfypxmbh.sHtML

[S11] C：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gnmnxxaou.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.fanxiaobao.xyz/Article/details/gcwfazeko.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gqgigcaeo.sHtML

fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/guyrbyvvf.sHtML

[S12] C：写文件
来源：http://baike.fanxiaobao.xyz/Article/details/gtbmmhixm.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.fanxiaobao.xyz/Article/details/gbcqkinbc.sHtML

[S13] C：宏定义
来源：http://www.share.fanxiaobao.xyz/Article/details/gautkxkvg.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fanxiaobao.xyz/Article/details/gkjiqnzit.sHtML

[S14] C：枚举
来源：http://3g.fanxiaobao.xyz/Article/details/gieehgsct.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.fanxiaobao.xyz/Article/details/ghxdkzwcw.sHtML

[S15] C：类型转换
来源：http://baike.fanxiaobao.xyz/Article/details/gbsaadxoh.sHtML

(double) a / b
来源：http://mobile.fanxiaobao.xyz/Article/details/gpkzqyiue.sHtML

[S16] C：位操作置位
来源：http://3g.fanxiaobao.xyz/Article/details/gnqiyidlo.sHtML

x |= (1 << 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gbpprkwnw.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gjbigpkvl.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.fanxiaobao.xyz/Article/details/gqifcznyv.sHtML

[S18] C：命令行参数
来源：http://wap.fanxiaobao.xyz/Article/details/gepcbzena.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbqmlrlmg.sHtML

[S19] C：快速排序
来源：http://baike.fanxiaobao.xyz/Article/details/gtbxylyuo.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyqyrsagy.sHtML

[S20] C：二分查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfyxciqfh.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjjxasqaq.sHtML

[S21] C：字符类别判断
来源：http://m.share.fanxiaobao.xyz/Article/details/ggsykratt.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fanxiaobao.xyz/Article/details/gsdarvajr.sHtML

[S22] C：字符串转数字
来源：http://read.share.fanxiaobao.xyz/Article/details/gmyyhvvrv.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gatvlsino.sHtML

[S23] C：随机数
来源：http://read.share.fanxiaobao.xyz/Article/details/gywkyqeqt.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fanxiaobao.xyz/Article/details/gzvkwjqtc.sHtML

[S24] C：获取本地时间
来源：http://read.share.fanxiaobao.xyz/Article/details/gsaacapyy.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.fanxiaobao.xyz/Article/details/gdkglucap.sHtML

[S25] C：内存拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gqfgmihma.sHtML

memcpy(dst, src, n);
来源：http://m.share.fanxiaobao.xyz/Article/details/gsjmrqrbl.sHtML

[S26] C：内存清零
来源：http://read.share.fanxiaobao.xyz/Article/details/gnsanwqmr.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fanxiaobao.xyz/Article/details/ggrbkgjhp.sHtML

[S27] C：定义常量
来源：http://wap.fanxiaobao.xyz/Article/details/ggxjznada.sHtML

const double PI = 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gqngqkfym.sHtML

[S28] C：静态变量
来源：http://wap.fanxiaobao.xyz/Article/details/gvqtwrbgw.sHtML

static int counter = 0;
来源：http://3g.fanxiaobao.xyz/Article/details/gffxmetul.sHtML

[S29] C：变参函数
来源：http://blog.fanxiaobao.xyz/Article/details/gcgsqious.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fanxiaobao.xyz/Article/details/gmuzoklwm.sHtML

[S30] C：头文件保护
来源：http://mobile.fanxiaobao.xyz/Article/details/gbvhpwrah.sHtML

#ifndef X_H
来源：http://3g.fanxiaobao.xyz/Article/details/gbloeyngv.sHtML

#define X_H
来源：http://blog.fanxiaobao.xyz/Article/details/gkwwdvpfg.sHtML

#endif
来源：http://baike.fanxiaobao.xyz/Article/details/gfcfrcove.sHtML

[S31] C++：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gnclsnmve.sHtML

#include <iostream>
来源：http://3g.fanxiaobao.xyz/Article/details/gyzhehfls.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gntjilmox.sHtML

[S32] C++：字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/grfuleoog.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fanxiaobao.xyz/Article/details/gpmaecfyf.sHtML

[S33] C++：vector 增删
来源：http://blog.fanxiaobao.xyz/Article/details/gylcgsvjo.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.fanxiaobao.xyz/Article/details/gqavrodek.sHtML

[S34] C++：遍历 vector
来源：http://blog.fanxiaobao.xyz/Article/details/glnjuaork.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gzpzjmezk.sHtML

[S35] C++：map
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghyvhpahu.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxibotqgp.sHtML

[S36] C++：unordered_map
来源：http://baike.fanxiaobao.xyz/Article/details/gqgogioer.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/ggsqhrbiy.sHtML

[S37] C++：set
来源：http://mobile.fanxiaobao.xyz/Article/details/gdyvoykyp.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.fanxiaobao.xyz/Article/details/gmelnrzzn.sHtML

[S38] C++：排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gqkfmhygl.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmhlalbmr.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gdcnrcuxa.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fanxiaobao.xyz/Article/details/goqqyumkb.sHtML

[S40] C++：查找元素
来源：http://wap.fanxiaobao.xyz/Article/details/gdpovrwib.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gisxljzyg.sHtML

[S41] C++：类与构造函数
来源：http://blog.fanxiaobao.xyz/Article/details/gbbqblkgu.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.fanxiaobao.xyz/Article/details/givyjcqqp.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gugvrsecv.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.fanxiaobao.xyz/Article/details/gnyvreork.sHtML

[S43] C++：智能指针
来源：http://read.share.fanxiaobao.xyz/Article/details/gfjgjfiwm.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.fanxiaobao.xyz/Article/details/gemdlyrue.sHtML

[S44] C++：引用传参
来源：http://m.share.fanxiaobao.xyz/Article/details/gwsrogjhk.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqfygyckt.sHtML

[S45] C++：lambda
来源：http://www.share.fanxiaobao.xyz/Article/details/gmtmxfnye.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/givtuyznr.sHtML

[S46] C++：函数模板
来源：http://mobile.fanxiaobao.xyz/Article/details/gnsdzmcxa.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gyyofiwls.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gmmdpmyvu.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.fanxiaobao.xyz/Article/details/gwzwcdndd.sHtML

[S48] C++：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gzdkyqsbw.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.fanxiaobao.xyz/Article/details/ghufdtpuo.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqxdpdnzg.sHtML

[S49] C++：写文件
来源：http://baike.fanxiaobao.xyz/Article/details/gyzjljzlb.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gesligujc.sHtML

[S50] C++：格式化数字
来源：http://blog.fanxiaobao.xyz/Article/details/gvlpawtos.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjvorlicg.sHtML

[S51] C++：显式类型转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gbdhpylhu.sHtML

static_cast<double>(a) / b
来源：http://mobile.fanxiaobao.xyz/Article/details/guyrhmeuq.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gczpmremu.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsffdeifx.sHtML

[S53] C++：移动语义
来源：http://m.share.fanxiaobao.xyz/Article/details/gyihactcv.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.fanxiaobao.xyz/Article/details/ggoffjiuy.sHtML

[S54] C++：异常处理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwqcziyfb.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gcjvqzyek.sHtML

[S55] C++：结构化绑定
来源：http://mobile.fanxiaobao.xyz/Article/details/ggrzsvvrz.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.fanxiaobao.xyz/Article/details/gvieozrgz.sHtML

[S56] C++：optional
来源：http://m.share.fanxiaobao.xyz/Article/details/gnnftfbpq.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.fanxiaobao.xyz/Article/details/gfhhsbkvu.sHtML

[S57] C++：编译期常量
来源：http://mobile.fanxiaobao.xyz/Article/details/gasdxfggu.sHtML

constexpr int N = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/gevjblhxc.sHtML

[S58] C++：命名空间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gypfdqzmf.sHtML


<!-- 参考信息 -->