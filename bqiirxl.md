代发 wailian999

name="${1:-default}"
来源：http://wap.fanxiaobao.xyz/Article/details/gxeqrepxe.sHtML

[R06] 判断命令是否存在
来源：http://www.share.fanxiaobao.xyz/Article/details/ghhnaimho.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gpngttdld.sHtML

[R07] if 判断文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gfttyrkcc.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gsxewnpzv.sHtML

[R08] 数值比较
来源：http://3g.fanxiaobao.xyz/Article/details/gbhrdxqwu.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gllooqijt.sHtML

[R09] 字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gcihbckgx.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/grjwyapiy.sHtML

[R10] 正则匹配
来源：http://baike.fanxiaobao.xyz/Article/details/gijwobwuz.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gnvjfpica.sHtML

[R11] case 多分支
来源：http://baike.fanxiaobao.xyz/Article/details/gzagbwkfl.sHtML

case "$1" in
来源：http://read.share.fanxiaobao.xyz/Article/details/gqykketld.sHtML

start) echo "启动" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gpucnupnm.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtkimrhhy.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/gnjnhsnwl.sHtML

esac
来源：http://wap.fanxiaobao.xyz/Article/details/gfyrqjelh.sHtML

[R12] for 遍历文件
来源：http://wap.fanxiaobao.xyz/Article/details/gmqdssxca.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gdrgsigth.sHtML

[R13] for 计数循环
来源：http://baike.fanxiaobao.xyz/Article/details/gbhzyjefz.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gbnqvsibd.sHtML

[R14] C 风格 for
来源：http://wap.fanxiaobao.xyz/Article/details/gvopvxqmf.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/ggthiomrh.sHtML

[R15] while 逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwdehoswo.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gblcrlczk.sHtML

[R16] until 等待条件
来源：http://mobile.fanxiaobao.xyz/Article/details/ghiapfony.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwgfxxnys.sHtML

[R17] 数组定义与取值
来源：http://m.share.fanxiaobao.xyz/Article/details/ggffpacok.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfwlszzyh.sHtML

[R18] 遍历数组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzbmzhzci.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkuhzwqml.sHtML

[R19] 数组长度
来源：http://blog.fanxiaobao.xyz/Article/details/gaifzswff.sHtML

echo "${#arr[@]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gsbdoubbd.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.fanxiaobao.xyz/Article/details/goclzxbwm.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gjzwkrqjp.sHtML

[R21] 字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gzooenowa.sHtML

echo "${#s}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gnfgmwzoa.sHtML

[R22] 截取子串
来源：http://m.share.fanxiaobao.xyz/Article/details/glgfsdfpm.sHtML

echo "${s:0:5}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gxrhalzuc.sHtML

[R23] 字符串替换
来源：http://m.share.fanxiaobao.xyz/Article/details/ghxupqebx.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.fanxiaobao.xyz/Article/details/gymjjxcrz.sHtML

[R24] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/gjgtcoumb.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gghtinivp.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.fanxiaobao.xyz/Article/details/grubxqsqa.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqojilvcl.sHtML

[R26] 命令替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gmphfdqzy.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwiygqngk.sHtML

[R27] 算术展开
来源：http://3g.fanxiaobao.xyz/Article/details/gauevxjaw.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.fanxiaobao.xyz/Article/details/gptauleag.sHtML

[R28] 浮点运算
来源：http://www.share.fanxiaobao.xyz/Article/details/gtmmzssfh.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fanxiaobao.xyz/Article/details/ghzoyklcw.sHtML

[R29] 定义函数
来源：http://mobile.fanxiaobao.xyz/Article/details/ghohybzsk.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fanxiaobao.xyz/Article/details/ghtofhoxm.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gylqdajkd.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.fanxiaobao.xyz/Article/details/gwkdupgni.sHtML

[R31] 局部变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grfrnaxhf.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggqahcvee.sHtML

[R32] 参数个数校验
来源：http://www.share.fanxiaobao.xyz/Article/details/gctgbonse.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gkhlfjnie.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.fanxiaobao.xyz/Article/details/gcoyaxvtt.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.fanxiaobao.xyz/Article/details/glaxygowz.sHtML

[R34] 退出时清理
来源：http://wap.fanxiaobao.xyz/Article/details/gcwcoizho.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/gtpyjzurf.sHtML

[R35] 后台执行并等待
来源：http://3g.fanxiaobao.xyz/Article/details/ghmtquwzi.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.fanxiaobao.xyz/Article/details/giaktuiav.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxxteitfi.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.fanxiaobao.xyz/Article/details/gpqbdstpq.sHtML

[R37] 把输出赋给变量
来源：http://3g.fanxiaobao.xyz/Article/details/gydnsifmt.sHtML

files=$(ls -1)
来源：http://baike.fanxiaobao.xyz/Article/details/gmvkfrwpi.sHtML

[R38] 管道串联
来源：http://www.share.fanxiaobao.xyz/Article/details/gvbbwwipx.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fanxiaobao.xyz/Article/details/gozlwwezu.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.fanxiaobao.xyz/Article/details/goygxyzrl.sHtML

cmd > out.log 2>&1
来源：http://read.share.fanxiaobao.xyz/Article/details/gcowarwdp.sHtML

[R40] 追加写日志
来源：http://baike.fanxiaobao.xyz/Article/details/gslhqnori.sHtML

echo "log" >> out.log
来源：http://mobile.fanxiaobao.xyz/Article/details/gxsacbgre.sHtML

[R41] 丢弃输出
来源：http://3g.fanxiaobao.xyz/Article/details/ghsxatumi.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/gjzyjaynp.sHtML

[R42] 输入重定向
来源：http://mobile.fanxiaobao.xyz/Article/details/ganvskxls.sHtML

wc -l < a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/glukrxila.sHtML

[R43] 按名字查找文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtsjlqrws.sHtML

find . -name "*.log" -type f
来源：http://blog.fanxiaobao.xyz/Article/details/gfwllhovy.sHtML

[R44] 按修改时间查找
来源：http://read.share.fanxiaobao.xyz/Article/details/gqexobnzh.sHtML

find . -mtime -7 -type f
来源：http://wap.fanxiaobao.xyz/Article/details/gtsqxdnxo.sHtML

[R45] 批量删除
来源：http://m.share.fanxiaobao.xyz/Article/details/glpmhhweb.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.fanxiaobao.xyz/Article/details/grkitrmjk.sHtML

[R46] 递归替换文件内容
来源：http://baike.fanxiaobao.xyz/Article/details/gnzfvthmw.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fanxiaobao.xyz/Article/details/gtwsiqmen.sHtML

[R47] sed 单行替换
来源：http://baike.fanxiaobao.xyz/Article/details/gidsporot.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gwvnhlgyq.sHtML

[R48] awk 取指定列
来源：http://blog.fanxiaobao.xyz/Article/details/gjghpmlbf.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gbxhhgedw.sHtML

[R49] awk 带条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gfpbgqfme.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.fanxiaobao.xyz/Article/details/gdvybfwcg.sHtML

[R50] awk 求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gxjogqrkk.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gkuybwttz.sHtML

[R51] 排序去重取前几
来源：http://3g.fanxiaobao.xyz/Article/details/gkvqserpm.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fanxiaobao.xyz/Article/details/giwwypcrd.sHtML

[R52] 统计行数
来源：http://read.share.fanxiaobao.xyz/Article/details/gxxglteap.sHtML

wc -l a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gembepwyz.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.fanxiaobao.xyz/Article/details/galbqmlax.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fanxiaobao.xyz/Article/details/gneqphfam.sHtML

[R54] 比较两个文件
来源：http://wap.fanxiaobao.xyz/Article/details/giaspzhdq.sHtML

diff a.txt b.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gzuzsgpin.sHtML

[R55] 压缩与解压
来源：http://read.share.fanxiaobao.xyz/Article/details/giyvtchwv.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fanxiaobao.xyz/Article/details/gshhbtife.sHtML

[R56] 远程拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gbrsvohfo.sHtML

scp file user@host:/path/
来源：http://blog.fanxiaobao.xyz/Article/details/grzfgudbv.sHtML

[R57] 远程执行命令
来源：http://mobile.fanxiaobao.xyz/Article/details/gmthikfei.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnikdxtsc.sHtML

[R58] 下载文件
来源：http://wap.fanxiaobao.xyz/Article/details/goehcdwkq.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fanxiaobao.xyz/Article/details/gkqrckppa.sHtML

[R59] 发 POST JSON
来源：http://baike.fanxiaobao.xyz/Article/details/gqwfduyhn.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fanxiaobao.xyz/Article/details/ghdjgoogl.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gbzzqoicv.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkqcdwwxr.sHtML

[R61] 磁盘占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gicsjrgbc.sHtML

df -h;  du -sh *
来源：http://www.share.fanxiaobao.xyz/Article/details/gmesfopxv.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/grgucekpt.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fanxiaobao.xyz/Article/details/gokuqtddr.sHtML

[R63] 内存与进程
来源：http://baike.fanxiaobao.xyz/Article/details/gqrbntaoq.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggtexpfic.sHtML

[R64] 结束进程
来源：http://m.share.fanxiaobao.xyz/Article/details/ghmrgeixk.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.fanxiaobao.xyz/Article/details/gbtrxcspb.sHtML

[R65] 查看端口占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gonyjqggj.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fanxiaobao.xyz/Article/details/gvddpyukv.sHtML

[R66] 定时任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtdfnxamt.sHtML

crontab -e;  crontab -l
来源：http://wap.fanxiaobao.xyz/Article/details/gakphmnry.sHtML

[R67] 生成随机十六进制串
来源：http://blog.fanxiaobao.xyz/Article/details/gfpwhyyxo.sHtML

openssl rand -hex 16
来源：http://read.share.fanxiaobao.xyz/Article/details/gsuqlphpp.sHtML

[R68] 计算文件校验值
来源：http://www.blog.fanxiaobao.xyz/Article/details/glxnmpyse.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/grifpieht.sHtML

[R69] 生成随机密码
来源：http://wap.fanxiaobao.xyz/Article/details/gqkuuogru.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fanxiaobao.xyz/Article/details/gblzqsylc.sHtML

[R70] 时间戳与互转
来源：http://www.share.fanxiaobao.xyz/Article/details/gttylnwoj.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fanxiaobao.xyz/Article/details/gqljcdrwj.sHtML

[R71] 日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gkkszczrt.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.fanxiaobao.xyz/Article/details/ggsoofnpk.sHtML

[R72] 等待端口就绪
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtvsqjayp.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkqnkcwih.sHtML

[R73] 分割大日志
来源：http://blog.fanxiaobao.xyz/Article/details/gkdagafgn.sHtML

split -l 1000 big.log part_
来源：http://read.share.fanxiaobao.xyz/Article/details/gnamghszy.sHtML

[R74] 批量重命名
来源：http://blog.fanxiaobao.xyz/Article/details/gskkscnpq.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.fanxiaobao.xyz/Article/details/ghgeashvx.sHtML

[R75] 导出环境变量
来源：http://www.share.fanxiaobao.xyz/Article/details/glwhdrybh.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fanxiaobao.xyz/Article/details/gkmdtjpsk.sHtML

[R76] 使用临时文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gzucxtaco.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/gvwvlxxqk.sHtML

[R77] 读取用户输入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvkoawudb.sHtML

read -rp "请输入: " ans
来源：http://3g.fanxiaobao.xyz/Article/details/gyxyzmgnl.sHtML

[R78] 交互式菜单
来源：http://read.share.fanxiaobao.xyz/Article/details/gndlxebin.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxngiyjev.sHtML

[R79] 解析命令行选项
来源：http://blog.fanxiaobao.xyz/Article/details/gxxnnleut.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.fanxiaobao.xyz/Article/details/gmhipndww.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fanxiaobao.xyz/Article/details/ghcsojwuo.sHtML

time ./run.sh
来源：http://read.share.fanxiaobao.xyz/Article/details/gbfoqaged.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gatmwywgh.sHtML

S. C / C++ 专题
来源：http://m.share.fanxiaobao.xyz/Article/details/gadsfvijs.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggcenumqd.sHtML

[S01] C：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gobpfntdw.sHtML

#include <stdio.h>
来源：http://baike.fanxiaobao.xyz/Article/details/gziqdaviy.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.fanxiaobao.xyz/Article/details/gjharfmyp.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggbhruqnm.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.fanxiaobao.xyz/Article/details/golyyqghg.sHtML

[S03] C：读入整数
来源：http://www.share.fanxiaobao.xyz/Article/details/gnvbkelvj.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcobcvgmg.sHtML

[S04] C：字符串复制
来源：http://baike.fanxiaobao.xyz/Article/details/ghjuhaikr.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.fanxiaobao.xyz/Article/details/gzsysptkv.sHtML

[S05] C：字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/ggwpapitv.sHtML

strlen(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqylaggew.sHtML

[S06] C：字符串比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gqkerazjv.sHtML

strcmp(a, b) == 0
来源：http://www.blog.fanxiaobao.xyz/Article/details/gijtffvtj.sHtML

[S07] C：数组遍历求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gwaggbcjy.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fanxiaobao.xyz/Article/details/ghlymqpyr.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fanxiaobao.xyz/Article/details/gwtmhxhqm.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fanxiaobao.xyz/Article/details/gfjvxmaha.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fanxiaobao.xyz/Article/details/gxitcoyav.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fanxiaobao.xyz/Article/details/gqvltwnbo.sHtML

[S10] C：指针与解引用
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghujcktlc.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fanxiaobao.xyz/Article/details/gjcbgxshq.sHtML

[S11] C：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gvandqtsn.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.fanxiaobao.xyz/Article/details/gjyevcczt.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gkvlsxbxw.sHtML

fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/glxuxrizz.sHtML

[S12] C：写文件
来源：http://3g.fanxiaobao.xyz/Article/details/grmacaypp.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/gryakkadp.sHtML

[S13] C：宏定义
来源：http://mobile.fanxiaobao.xyz/Article/details/gxxgsrkcj.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.fanxiaobao.xyz/Article/details/gzainaodw.sHtML

[S14] C：枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/gozfsbyrj.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.fanxiaobao.xyz/Article/details/gwfyakadd.sHtML

[S15] C：类型转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaacveecb.sHtML

(double) a / b
来源：http://m.share.fanxiaobao.xyz/Article/details/gvgwmlpuv.sHtML

[S16] C：位操作置位
来源：http://blog.fanxiaobao.xyz/Article/details/gtujjjwfz.sHtML

x |= (1 << 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gksmerbgf.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggzsrtfmt.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.fanxiaobao.xyz/Article/details/gzqabdgby.sHtML

[S18] C：命令行参数
来源：http://baike.fanxiaobao.xyz/Article/details/gsfjaltta.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwqogoqob.sHtML

[S19] C：快速排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxpixkttk.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gypczrlrb.sHtML

[S20] C：二分查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsjxtzgsq.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/gdobtpzdn.sHtML

[S21] C：字符类别判断
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdcvoceut.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fanxiaobao.xyz/Article/details/ggbcbuunz.sHtML

[S22] C：字符串转数字
来源：http://blog.fanxiaobao.xyz/Article/details/giucrvoom.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.fanxiaobao.xyz/Article/details/gznywwzld.sHtML

[S23] C：随机数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggufmkofe.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpudnyyty.sHtML

[S24] C：获取本地时间
来源：http://read.share.fanxiaobao.xyz/Article/details/glqagtwis.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ginzznrij.sHtML

[S25] C：内存拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/gmdfwxdob.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fanxiaobao.xyz/Article/details/grkftxour.sHtML

[S26] C：内存清零
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzsbolhbb.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.fanxiaobao.xyz/Article/details/gezwdlkkw.sHtML

[S27] C：定义常量
来源：http://baike.fanxiaobao.xyz/Article/details/geijkguso.sHtML

const double PI = 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gbbvaslrf.sHtML

[S28] C：静态变量
来源：http://3g.fanxiaobao.xyz/Article/details/gshmlhexf.sHtML

static int counter = 0;
来源：http://m.share.fanxiaobao.xyz/Article/details/ggppvbxnj.sHtML

[S29] C：变参函数
来源：http://baike.fanxiaobao.xyz/Article/details/grvlktufq.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fanxiaobao.xyz/Article/details/ggtprcint.sHtML

[S30] C：头文件保护
来源：http://m.share.fanxiaobao.xyz/Article/details/gxdumaqdy.sHtML

#ifndef X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/gdjpcfaxa.sHtML

#define X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/gzfxggpey.sHtML

#endif
来源：http://3g.fanxiaobao.xyz/Article/details/gumkzofaz.sHtML

[S31] C++：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gvgdkqmbd.sHtML

#include <iostream>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfafjzbya.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gqzzsbwkb.sHtML

[S32] C++：字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gzrevdqmm.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.fanxiaobao.xyz/Article/details/gvkhtdgnl.sHtML

[S33] C++：vector 增删
来源：http://baike.fanxiaobao.xyz/Article/details/ghkbiibrg.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gyenkskuu.sHtML

[S34] C++：遍历 vector
来源：http://read.share.fanxiaobao.xyz/Article/details/ghzwefmwy.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gsrhypppu.sHtML

[S35] C++：map
来源：http://m.share.fanxiaobao.xyz/Article/details/gumikhuzz.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/glbkicbdp.sHtML

[S36] C++：unordered_map
来源：http://mobile.fanxiaobao.xyz/Article/details/gctvuhccb.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gtvibuwef.sHtML

[S37] C++：set
来源：http://wap.fanxiaobao.xyz/Article/details/guuadrdrz.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gwdqsdfuo.sHtML

[S38] C++：排序
来源：http://baike.fanxiaobao.xyz/Article/details/gquxuomyi.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.fanxiaobao.xyz/Article/details/ggccrhjrh.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.fanxiaobao.xyz/Article/details/guszivilf.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtwlkrtzg.sHtML

[S40] C++：查找元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gjqevbrwz.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gxeqnyhjv.sHtML

[S41] C++：类与构造函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gpqizngrz.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fanxiaobao.xyz/Article/details/gzqlmkpbi.sHtML

[S42] C++：继承与虚函数
来源：http://blog.fanxiaobao.xyz/Article/details/gyxuspqtl.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.fanxiaobao.xyz/Article/details/gpjzrsxnj.sHtML

[S43] C++：智能指针
来源：http://read.share.fanxiaobao.xyz/Article/details/gslqwjjyh.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fanxiaobao.xyz/Article/details/gxntwkyfb.sHtML

[S44] C++：引用传参
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwccvhkxs.sHtML

void inc(int &x) { ++x; }
来源：http://wap.fanxiaobao.xyz/Article/details/ggdndnkdy.sHtML

[S45] C++：lambda
来源：http://baike.fanxiaobao.xyz/Article/details/gupipkgah.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gtitlwuhr.sHtML

[S46] C++：函数模板
来源：http://wap.fanxiaobao.xyz/Article/details/gfkuoxwqb.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gjrbkwezy.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gqrwvvkzv.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfqliaynb.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmjuyhxrz.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.fanxiaobao.xyz/Article/details/gzrupbkor.sHtML

while (std::getline(in, line)) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gbffwlfhs.sHtML

[S49] C++：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/gfujabeve.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.fanxiaobao.xyz/Article/details/gycbbueqt.sHtML

[S50] C++：格式化数字
来源：http://3g.fanxiaobao.xyz/Article/details/gourvdach.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/gdyxyssio.sHtML

[S51] C++：显式类型转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gocdzoxoa.sHtML

static_cast<double>(a) / b
来源：http://baike.fanxiaobao.xyz/Article/details/gplhgzycd.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.fanxiaobao.xyz/Article/details/gslwudsgn.sHtML

int size() const noexcept { return n_; }
来源：http://wap.fanxiaobao.xyz/Article/details/guvdufugg.sHtML

[S53] C++：移动语义
来源：http://read.share.fanxiaobao.xyz/Article/details/guiivoppk.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxvnyexnd.sHtML

[S54] C++：异常处理
来源：http://blog.fanxiaobao.xyz/Article/details/gubnnopdw.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/guyszickr.sHtML

[S55] C++：结构化绑定
来源：http://baike.fanxiaobao.xyz/Article/details/goghacpcj.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.fanxiaobao.xyz/Article/details/gguivdbcf.sHtML

[S56] C++：optional
来源：http://wap.fanxiaobao.xyz/Article/details/gylemqccz.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gukrvxwch.sHtML

[S57] C++：编译期常量
来源：http://m.share.fanxiaobao.xyz/Article/details/grqqckakz.sHtML

constexpr int N = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/gdplddois.sHtML

[S58] C++：命名空间
来源：http://mobile.fanxiaobao.xyz/Article/details/grlxtanhy.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.fanxiaobao.xyz/Article/details/gborqxtrs.sHtML

[S59] C++：静态断言
来源：http://www.blog.fanxiaobao.xyz/Article/details/gukbaomch.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.fanxiaobao.xyz/Article/details/gejotlwab.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcvnovmnx.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxxjglfkr.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gbhmzpxdx.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkvrtfgdo.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsgjsrrux.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gqucyokln.sHtML

println("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/gevvffppr.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnzutafwd.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.fanxiaobao.xyz/Article/details/gjianlpcl.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.fanxiaobao.xyz/Article/details/gpqaagsae.sHtML

"值: $b"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnzectrwa.sHtML

[T04] Kotlin：空安全
来源：http://wap.fanxiaobao.xyz/Article/details/gkmomuqcc.sHtML

val n: String? = null;  n?.length
来源：http://blog.fanxiaobao.xyz/Article/details/gpuxrmsuk.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/gzsyaewfa.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.fanxiaobao.xyz/Article/details/gydfnmtqq.sHtML

[T06] Kotlin：集合映射
来源：http://baike.fanxiaobao.xyz/Article/details/gxoohbsou.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gmtqwmqln.sHtML


<!-- 参考信息 -->