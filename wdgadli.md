代发 wailian999

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gwauzdekl.sHtML

[R10] 正则匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gqfwibkbr.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gfixyligz.sHtML

[R11] case 多分支
来源：http://3g.fanxiaobao.xyz/Article/details/gpprgnakj.sHtML

case "$1" in
来源：http://www.share.fanxiaobao.xyz/Article/details/gjbpgnbfj.sHtML

start) echo "启动" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghngzoqmm.sHtML

stop)  echo "停止" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/gmygygckt.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gbdburorp.sHtML

esac
来源：http://www.share.fanxiaobao.xyz/Article/details/gmohfnkir.sHtML

[R12] for 遍历文件
来源：http://blog.fanxiaobao.xyz/Article/details/gujientyk.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfvelylqi.sHtML

[R13] for 计数循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gqzvkppcw.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/getygtipd.sHtML

[R14] C 风格 for
来源：http://m.share.fanxiaobao.xyz/Article/details/gujiopdio.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/ghypzuzzb.sHtML

[R15] while 逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gwlrlkcno.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gyjmhpncw.sHtML

[R16] until 等待条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gnmrdpbit.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gouxpztnf.sHtML

[R17] 数组定义与取值
来源：http://3g.fanxiaobao.xyz/Article/details/gvhdzgtcs.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/ganrdsfou.sHtML

[R18] 遍历数组
来源：http://www.share.fanxiaobao.xyz/Article/details/gysdincgf.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gxnckrluv.sHtML

[R19] 数组长度
来源：http://read.share.fanxiaobao.xyz/Article/details/ggfwcshbs.sHtML

echo "${#arr[@]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gmuhsnheh.sHtML

[R20] 关联数组（字典）
来源：http://baike.fanxiaobao.xyz/Article/details/gzvepjsac.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gigrknfvo.sHtML

[R21] 字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/goipszwul.sHtML

echo "${#s}"
来源：http://mobile.fanxiaobao.xyz/Article/details/grxihrzwm.sHtML

[R22] 截取子串
来源：http://m.share.fanxiaobao.xyz/Article/details/gwkfigyyp.sHtML

echo "${s:0:5}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gljiztljw.sHtML

[R23] 字符串替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guvtwieme.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.fanxiaobao.xyz/Article/details/glcrtmzrv.sHtML

[R24] 大小写转换
来源：http://blog.fanxiaobao.xyz/Article/details/gvmqjzrnv.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.fanxiaobao.xyz/Article/details/ghjrryecm.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.fanxiaobao.xyz/Article/details/gypegoaox.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsqjlwfwf.sHtML

[R26] 命令替换
来源：http://baike.fanxiaobao.xyz/Article/details/gtvjzsluh.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.fanxiaobao.xyz/Article/details/glsepuqry.sHtML

[R27] 算术展开
来源：http://wap.fanxiaobao.xyz/Article/details/gpbocktin.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.fanxiaobao.xyz/Article/details/gcqdqkxqf.sHtML

[R28] 浮点运算
来源：http://blog.fanxiaobao.xyz/Article/details/gkjiaowsz.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fanxiaobao.xyz/Article/details/gdyaailwd.sHtML

[R29] 定义函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gcrdzptax.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.fanxiaobao.xyz/Article/details/gfdlunfhw.sHtML

[R30] 函数返回状态码
来源：http://blog.fanxiaobao.xyz/Article/details/gqtjwejzs.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fanxiaobao.xyz/Article/details/gmuizdsni.sHtML

[R31] 局部变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gtqblvdxk.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gbtonzzil.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvgldsxmn.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqijiiohh.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.fanxiaobao.xyz/Article/details/guhkgrfmk.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.fanxiaobao.xyz/Article/details/gljpiojxn.sHtML

[R34] 退出时清理
来源：http://m.share.fanxiaobao.xyz/Article/details/gptfwtkvi.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/gkmokfsac.sHtML

[R35] 后台执行并等待
来源：http://wap.fanxiaobao.xyz/Article/details/gervzjovh.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.fanxiaobao.xyz/Article/details/glzslptcr.sHtML

[R36] 并发执行多个任务
来源：http://blog.fanxiaobao.xyz/Article/details/gdrfervvd.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fanxiaobao.xyz/Article/details/ghlapivlm.sHtML

[R37] 把输出赋给变量
来源：http://3g.fanxiaobao.xyz/Article/details/gbbbwikxw.sHtML

files=$(ls -1)
来源：http://baike.fanxiaobao.xyz/Article/details/gshbsktqv.sHtML

[R38] 管道串联
来源：http://mobile.fanxiaobao.xyz/Article/details/gelcipgrl.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.fanxiaobao.xyz/Article/details/gficizmgj.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fanxiaobao.xyz/Article/details/gmstxykuh.sHtML

cmd > out.log 2>&1
来源：http://www.blog.fanxiaobao.xyz/Article/details/goyahkfgt.sHtML

[R40] 追加写日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtsfrtnyu.sHtML

echo "log" >> out.log
来源：http://3g.fanxiaobao.xyz/Article/details/gpperyjph.sHtML

[R41] 丢弃输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxtsaeulh.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyrfzfbtp.sHtML

[R42] 输入重定向
来源：http://read.share.fanxiaobao.xyz/Article/details/gcyswfnxa.sHtML

wc -l < a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gedmfurey.sHtML

[R43] 按名字查找文件
来源：http://baike.fanxiaobao.xyz/Article/details/ghmhldfvu.sHtML

find . -name "*.log" -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/glnypbhmh.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtpdrzdpa.sHtML

find . -mtime -7 -type f
来源：http://read.share.fanxiaobao.xyz/Article/details/gfafdftfi.sHtML

[R45] 批量删除
来源：http://www.share.fanxiaobao.xyz/Article/details/gmngrujok.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.fanxiaobao.xyz/Article/details/gloksrnab.sHtML

[R46] 递归替换文件内容
来源：http://www.share.fanxiaobao.xyz/Article/details/ghowycwcg.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fanxiaobao.xyz/Article/details/grkodgymg.sHtML

[R47] sed 单行替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkpfhlovc.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gwpfeaebb.sHtML

[R48] awk 取指定列
来源：http://read.share.fanxiaobao.xyz/Article/details/gpxthdkrw.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gaecezxkq.sHtML

[R49] awk 带条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gonptvxbg.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.fanxiaobao.xyz/Article/details/gzzhtlyxj.sHtML

[R50] awk 求和
来源：http://blog.fanxiaobao.xyz/Article/details/gmwwclyjp.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/ghvxmqrnu.sHtML

[R51] 排序去重取前几
来源：http://www.share.fanxiaobao.xyz/Article/details/gksomzdqk.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.fanxiaobao.xyz/Article/details/gnjfcrxng.sHtML

[R52] 统计行数
来源：http://read.share.fanxiaobao.xyz/Article/details/gbexlxbsg.sHtML

wc -l a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gqbjtjpbf.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.fanxiaobao.xyz/Article/details/giiafkasy.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fanxiaobao.xyz/Article/details/gmpwbqluz.sHtML

[R54] 比较两个文件
来源：http://3g.fanxiaobao.xyz/Article/details/gsvslldyc.sHtML

diff a.txt b.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gpxbyzapw.sHtML

[R55] 压缩与解压
来源：http://blog.fanxiaobao.xyz/Article/details/gmqizkjxp.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwesqafzt.sHtML

[R56] 远程拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gcjqryiwf.sHtML

scp file user@host:/path/
来源：http://www.share.fanxiaobao.xyz/Article/details/goemvruzx.sHtML

[R57] 远程执行命令
来源：http://www.blog.fanxiaobao.xyz/Article/details/gicaccowg.sHtML

ssh user@host 'uptime'
来源：http://3g.fanxiaobao.xyz/Article/details/guveqbqsw.sHtML

[R58] 下载文件
来源：http://baike.fanxiaobao.xyz/Article/details/gexhddrem.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.fanxiaobao.xyz/Article/details/ggcplepkm.sHtML

[R59] 发 POST JSON
来源：http://mobile.fanxiaobao.xyz/Article/details/ggtdisxpi.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.fanxiaobao.xyz/Article/details/gavndcggh.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.fanxiaobao.xyz/Article/details/goumymrgq.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fanxiaobao.xyz/Article/details/gzoxhrvgd.sHtML

[R61] 磁盘占用
来源：http://3g.fanxiaobao.xyz/Article/details/glfjyzayx.sHtML

df -h;  du -sh *
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfsopslrg.sHtML

[R62] 找最占空间的文件
来源：http://wap.fanxiaobao.xyz/Article/details/glpiamfno.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fanxiaobao.xyz/Article/details/gbjjlpcfa.sHtML

[R63] 内存与进程
来源：http://wap.fanxiaobao.xyz/Article/details/gkbmbntaz.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.fanxiaobao.xyz/Article/details/gndwgrovt.sHtML

[R64] 结束进程
来源：http://blog.fanxiaobao.xyz/Article/details/gzzgaqqiy.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fanxiaobao.xyz/Article/details/gamwugpvv.sHtML

[R65] 查看端口占用
来源：http://3g.fanxiaobao.xyz/Article/details/gbwabxmdy.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.fanxiaobao.xyz/Article/details/gdezrbmlh.sHtML

[R66] 定时任务
来源：http://3g.fanxiaobao.xyz/Article/details/gtafxoaew.sHtML

crontab -e;  crontab -l
来源：http://www.share.fanxiaobao.xyz/Article/details/gznudlhct.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fanxiaobao.xyz/Article/details/gyysfivmy.sHtML

openssl rand -hex 16
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsmkbseyi.sHtML

[R68] 计算文件校验值
来源：http://www.share.fanxiaobao.xyz/Article/details/gjrexbjhp.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gtwqdpcji.sHtML

[R69] 生成随机密码
来源：http://mobile.fanxiaobao.xyz/Article/details/gqckoefgx.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fanxiaobao.xyz/Article/details/ghconbtkg.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghinyjufu.sHtML

date +%s;  date -d @1700000000
来源：http://blog.fanxiaobao.xyz/Article/details/gvfrdjogr.sHtML

[R71] 日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gipdhrriu.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gekfxwmnr.sHtML

[R72] 等待端口就绪
来源：http://3g.fanxiaobao.xyz/Article/details/ghiosxgnf.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcvglwqrf.sHtML

[R73] 分割大日志
来源：http://mobile.fanxiaobao.xyz/Article/details/govapodjm.sHtML

split -l 1000 big.log part_
来源：http://www.share.fanxiaobao.xyz/Article/details/ggyxugqhd.sHtML

[R74] 批量重命名
来源：http://www.blog.fanxiaobao.xyz/Article/details/goczhpogy.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gntohzsxg.sHtML

[R75] 导出环境变量
来源：http://baike.fanxiaobao.xyz/Article/details/gjyzwwpvx.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fanxiaobao.xyz/Article/details/goswmvtxz.sHtML

[R76] 使用临时文件
来源：http://baike.fanxiaobao.xyz/Article/details/gjuywvlwy.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/gwxpoyavy.sHtML

[R77] 读取用户输入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghtqkcjoi.sHtML

read -rp "请输入: " ans
来源：http://m.share.fanxiaobao.xyz/Article/details/gdqhyoqns.sHtML

[R78] 交互式菜单
来源：http://www.share.fanxiaobao.xyz/Article/details/gdarbqkzw.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gycxpzvsp.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gceafmfka.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gbwbaqcpx.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fanxiaobao.xyz/Article/details/gquvfzdlm.sHtML

time ./run.sh
来源：http://www.blog.fanxiaobao.xyz/Article/details/guohbzxdq.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gutpdtent.sHtML

S. C / C++ 专题
来源：http://m.share.fanxiaobao.xyz/Article/details/gqazcwmzr.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghwfbvjuf.sHtML

[S01] C：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gdabuqjsu.sHtML

#include <stdio.h>
来源：http://blog.fanxiaobao.xyz/Article/details/gbnmuilsb.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gtlmadgci.sHtML

[S02] C：变量与格式化输出
来源：http://blog.fanxiaobao.xyz/Article/details/gkxlbedqi.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.fanxiaobao.xyz/Article/details/gjvarligi.sHtML

[S03] C：读入整数
来源：http://3g.fanxiaobao.xyz/Article/details/guquqrqja.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fanxiaobao.xyz/Article/details/gwubjrvlu.sHtML

[S04] C：字符串复制
来源：http://mobile.fanxiaobao.xyz/Article/details/gnlmrtqnz.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.fanxiaobao.xyz/Article/details/gpulmsowb.sHtML

[S05] C：字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gamsvnkar.sHtML

strlen(s)
来源：http://wap.fanxiaobao.xyz/Article/details/ghxdsnjdy.sHtML

[S06] C：字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/gbsbcfkjp.sHtML

strcmp(a, b) == 0
来源：http://baike.fanxiaobao.xyz/Article/details/gtcgnilsb.sHtML

[S07] C：数组遍历求和
来源：http://blog.fanxiaobao.xyz/Article/details/gaaawfiws.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.fanxiaobao.xyz/Article/details/gpfwiqtog.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghjmhsaxk.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.fanxiaobao.xyz/Article/details/gpfdctnrf.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.fanxiaobao.xyz/Article/details/gzeiesfjg.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqubvbvdv.sHtML

[S10] C：指针与解引用
来源：http://read.share.fanxiaobao.xyz/Article/details/gdvujhwxv.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gipnjwhyi.sHtML

[S11] C：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gtguwcvnl.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.fanxiaobao.xyz/Article/details/gifxvvrji.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gdagyisiw.sHtML

fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/gmrzyqypo.sHtML

[S12] C：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gfynhnugv.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwnzajbgq.sHtML

[S13] C：宏定义
来源：http://m.share.fanxiaobao.xyz/Article/details/gmwebpied.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.fanxiaobao.xyz/Article/details/gsbmsqrps.sHtML

[S14] C：枚举
来源：http://baike.fanxiaobao.xyz/Article/details/gouozyaes.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fanxiaobao.xyz/Article/details/gmkpqkfwb.sHtML

[S15] C：类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/gimngxdrc.sHtML

(double) a / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqjbundvb.sHtML

[S16] C：位操作置位
来源：http://wap.fanxiaobao.xyz/Article/details/gvqycaeqh.sHtML

x |= (1 << 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtdhwwyol.sHtML

[S17] C：安全拼接字符串
来源：http://blog.fanxiaobao.xyz/Article/details/ggthgrvcx.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.fanxiaobao.xyz/Article/details/gwlphzkmk.sHtML

[S18] C：命令行参数
来源：http://blog.fanxiaobao.xyz/Article/details/grwohubch.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghccplprz.sHtML

[S19] C：快速排序
来源：http://baike.fanxiaobao.xyz/Article/details/gyivxraii.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/gylkdbfvi.sHtML

[S20] C：二分查找
来源：http://mobile.fanxiaobao.xyz/Article/details/guruybxrc.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/gnitecdax.sHtML

[S21] C：字符类别判断
来源：http://blog.fanxiaobao.xyz/Article/details/guyjfymht.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.fanxiaobao.xyz/Article/details/gjnbyiljg.sHtML

[S22] C：字符串转数字
来源：http://www.share.fanxiaobao.xyz/Article/details/gsmcophiu.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.fanxiaobao.xyz/Article/details/gbpjzncoj.sHtML

[S23] C：随机数
来源：http://m.share.fanxiaobao.xyz/Article/details/gulmlcxfs.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.fanxiaobao.xyz/Article/details/gvvrczbap.sHtML

[S24] C：获取本地时间
来源：http://www.share.fanxiaobao.xyz/Article/details/gesrbumqf.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fanxiaobao.xyz/Article/details/gtluomatq.sHtML

[S25] C：内存拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gzyrrnlsw.sHtML

memcpy(dst, src, n);
来源：http://3g.fanxiaobao.xyz/Article/details/gbqugsvri.sHtML

[S26] C：内存清零
来源：http://m.share.fanxiaobao.xyz/Article/details/gziigwzri.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmcxfnvjl.sHtML

[S27] C：定义常量
来源：http://baike.fanxiaobao.xyz/Article/details/gwjyfbnoo.sHtML

const double PI = 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcjhprtir.sHtML

[S28] C：静态变量
来源：http://3g.fanxiaobao.xyz/Article/details/gljmpfngv.sHtML

static int counter = 0;
来源：http://mobile.fanxiaobao.xyz/Article/details/gropfsigt.sHtML

[S29] C：变参函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gioxtosvm.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fanxiaobao.xyz/Article/details/gwjdesdyh.sHtML

[S30] C：头文件保护
来源：http://read.share.fanxiaobao.xyz/Article/details/gmnubdcbz.sHtML

#ifndef X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/gsrjyebyi.sHtML

#define X_H
来源：http://blog.fanxiaobao.xyz/Article/details/gbgbdhgwi.sHtML

#endif
来源：http://blog.fanxiaobao.xyz/Article/details/gprvanegw.sHtML

[S31] C++：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/glwqpbmco.sHtML

#include <iostream>
来源：http://3g.fanxiaobao.xyz/Article/details/gbgbsbvoq.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbzycjmvk.sHtML

[S32] C++：字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gsngkpgze.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fanxiaobao.xyz/Article/details/gdbfwdmqz.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fanxiaobao.xyz/Article/details/govefmokq.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzdpuxmgz.sHtML

[S34] C++：遍历 vector
来源：http://mobile.fanxiaobao.xyz/Article/details/gnhhxdlyu.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.fanxiaobao.xyz/Article/details/ginpzgapp.sHtML

[S35] C++：map
来源：http://3g.fanxiaobao.xyz/Article/details/gstppfalf.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gxvczbscq.sHtML

[S36] C++：unordered_map
来源：http://3g.fanxiaobao.xyz/Article/details/gjhvxlsmv.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gxiyfqcug.sHtML

[S37] C++：set
来源：http://wap.fanxiaobao.xyz/Article/details/gjpzdlvtm.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/ghapvrlyx.sHtML

[S38] C++：排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gaavsamij.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghmzcdksk.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.fanxiaobao.xyz/Article/details/gvntyvhni.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fanxiaobao.xyz/Article/details/gjnfhpfft.sHtML

[S40] C++：查找元素
来源：http://wap.fanxiaobao.xyz/Article/details/gylxgyqcm.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gctarodxu.sHtML

[S41] C++：类与构造函数
来源：http://read.share.fanxiaobao.xyz/Article/details/getnmcqkl.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fanxiaobao.xyz/Article/details/ggjqsmvjr.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gtqcdbcgy.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.fanxiaobao.xyz/Article/details/gwfdiuneo.sHtML

[S43] C++：智能指针
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gahjrmhoj.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.fanxiaobao.xyz/Article/details/gonfuggma.sHtML

[S44] C++：引用传参
来源：http://baike.fanxiaobao.xyz/Article/details/ggirijohj.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbkamsuof.sHtML

[S45] C++：lambda
来源：http://blog.fanxiaobao.xyz/Article/details/gygkblyal.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.fanxiaobao.xyz/Article/details/ggyorbtij.sHtML

[S46] C++：函数模板
来源：http://m.share.fanxiaobao.xyz/Article/details/ggpkbiish.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnrbfzpfr.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gbwaqcaih.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gmqpihiwu.sHtML

[S48] C++：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gdnsvbbgs.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.fanxiaobao.xyz/Article/details/gcpszaoat.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnxpwahlg.sHtML

[S49] C++：写文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gquztkgcx.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fanxiaobao.xyz/Article/details/gbwazesqn.sHtML

[S50] C++：格式化数字
来源：http://3g.fanxiaobao.xyz/Article/details/gqefadgkz.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/gdopeyqeg.sHtML

[S51] C++：显式类型转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gqyxdsplw.sHtML

static_cast<double>(a) / b
来源：http://baike.fanxiaobao.xyz/Article/details/gmtpxmoqs.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.fanxiaobao.xyz/Article/details/gzwmyeqjg.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gkimocoef.sHtML

[S53] C++：移动语义
来源：http://wap.fanxiaobao.xyz/Article/details/gozsmddin.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.fanxiaobao.xyz/Article/details/gxmhxbufi.sHtML

[S54] C++：异常处理
来源：http://blog.fanxiaobao.xyz/Article/details/grlzpwpgf.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gidkrpxty.sHtML

[S55] C++：结构化绑定
来源：http://wap.fanxiaobao.xyz/Article/details/gosxinejq.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.fanxiaobao.xyz/Article/details/gcdyduuxc.sHtML

[S56] C++：optional
来源：http://m.share.fanxiaobao.xyz/Article/details/ghdaetumo.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gsqvmsobu.sHtML

[S57] C++：编译期常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gutenlapr.sHtML

constexpr int N = 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/gennulrmp.sHtML

[S58] C++：命名空间
来源：http://read.share.fanxiaobao.xyz/Article/details/gxubhywup.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gglzcgabz.sHtML

[S59] C++：静态断言
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkhfjfzdu.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fanxiaobao.xyz/Article/details/gusbsnjjq.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gpuwenyil.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.fanxiaobao.xyz/Article/details/gnuiwcgzd.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gluzcotfg.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fanxiaobao.xyz/Article/details/gefrcajnp.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gbrkfiaom.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gumclptnv.sHtML

println("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gdairqlrh.sHtML

[T02] Kotlin：变量
来源：http://3g.fanxiaobao.xyz/Article/details/gjtbitbzv.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.fanxiaobao.xyz/Article/details/gbqjdccjx.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gylmlgxjs.sHtML

"值: $b"
来源：http://www.share.fanxiaobao.xyz/Article/details/gqfjcutrb.sHtML

[T04] Kotlin：空安全
来源：http://m.share.fanxiaobao.xyz/Article/details/ggihjaehx.sHtML

val n: String? = null;  n?.length
来源：http://3g.fanxiaobao.xyz/Article/details/guhkijsoz.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxzhzyecr.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggzgftptf.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.fanxiaobao.xyz/Article/details/gltzxkknb.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.fanxiaobao.xyz/Article/details/gchptbthr.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glnmmpnvt.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggexvdorp.sHtML

[T08] Kotlin：数据类
来源：http://wap.fanxiaobao.xyz/Article/details/gakxivvdc.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnjqgkvgz.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gslcjscys.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.fanxiaobao.xyz/Article/details/glmsyrvsx.sHtML

[T10] Kotlin：默认参数
来源：http://blog.fanxiaobao.xyz/Article/details/gvfmncfqm.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.fanxiaobao.xyz/Article/details/gsresumjt.sHtML


<!-- 参考信息 -->