代发 wailian999

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.hesvh.cn/Article/details/goklfjwvu.sHtML

[R08] 数值比较
来源：http://mobile.hesvh.cn/Article/details/gdkzukyhu.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gvkjzwdtq.sHtML

[R09] 字符串比较
来源：http://www.share.fehbvm.com/Article/details/grnzemvlg.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gjrwhroni.sHtML

[R10] 正则匹配
来源：http://baike.zdbjq.cn/Article/details/gsxqyauft.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.hesvh.cn/Article/details/genidxqrd.sHtML

[R11] case 多分支
来源：http://wap.fehbvm.com/Article/details/guolueaix.sHtML

case "$1" in
来源：http://www.share.fehbvm.com/Article/details/gyejnzntu.sHtML

start) echo "启动" ;;
来源：http://m.share.zdbjq.cn/Article/details/gtovuqbms.sHtML

stop)  echo "停止" ;;
来源：http://blog.zdbjq.cn/Article/details/glmwshbot.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.fehbvm.com/Article/details/gafkkmeca.sHtML

esac
来源：http://m.share.zdbjq.cn/Article/details/gzyjzjpit.sHtML

[R12] for 遍历文件
来源：http://wap.fehbvm.com/Article/details/ggevzezim.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.hesvh.cn/Article/details/gnrrsucyd.sHtML

[R13] for 计数循环
来源：http://www.share.fehbvm.com/Article/details/ghyqbpyto.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.zdbjq.cn/Article/details/goubuyhzd.sHtML

[R14] C 风格 for
来源：http://mobile.zdbjq.cn/Article/details/gfcecckwd.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.hesvh.cn/Article/details/gnggjaqut.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gznpcfpel.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.zdbjq.cn/Article/details/gxjuzxbqv.sHtML

[R16] until 等待条件
来源：http://www.blog.zdbjq.cn/Article/details/gtwidnasw.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.hesvh.cn/Article/details/ghwkintoq.sHtML

[R17] 数组定义与取值
来源：http://m.share.fehbvm.com/Article/details/ggmyruoza.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.hesvh.cn/Article/details/gjkmccyua.sHtML

[R18] 遍历数组
来源：http://mobile.hesvh.cn/Article/details/gdxjrxxbh.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.fehbvm.com/Article/details/gpgpgtnkk.sHtML

[R19] 数组长度
来源：http://www.share.hesvh.cn/Article/details/gjcaymihk.sHtML

echo "${#arr[@]}"
来源：http://wap.hesvh.cn/Article/details/gpykierez.sHtML

[R20] 关联数组（字典）
来源：http://www.share.fehbvm.com/Article/details/gcdgghdpm.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.zdbjq.cn/Article/details/gxqxluvrr.sHtML

[R21] 字符串长度
来源：http://blog.fehbvm.com/Article/details/gbldxahtw.sHtML

echo "${#s}"
来源：http://mobile.hesvh.cn/Article/details/gmwdgocbi.sHtML

[R22] 截取子串
来源：http://wap.hesvh.cn/Article/details/gudtojahn.sHtML

echo "${s:0:5}"
来源：http://www.blog.fehbvm.com/Article/details/gqtoufzmy.sHtML

[R23] 字符串替换
来源：http://mobile.fehbvm.com/Article/details/gmromcpfb.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.zdbjq.cn/Article/details/gviygoeju.sHtML

[R24] 大小写转换
来源：http://read.share.fehbvm.com/Article/details/gyisuxpmx.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.hesvh.cn/Article/details/gmwxkqhyw.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.zdbjq.cn/Article/details/gywtuldji.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fehbvm.com/Article/details/grtqbflcq.sHtML

[R26] 命令替换
来源：http://read.share.zdbjq.cn/Article/details/gjxwzuzjh.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.zdbjq.cn/Article/details/gqmtmfsgv.sHtML

[R27] 算术展开
来源：http://blog.fehbvm.com/Article/details/ggfiaxdte.sHtML

echo $((1 + 2 * 3))
来源：http://blog.zdbjq.cn/Article/details/gbuccazhj.sHtML

[R28] 浮点运算
来源：http://wap.hesvh.cn/Article/details/gucfukbmz.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.fehbvm.com/Article/details/gnllquvoe.sHtML

[R29] 定义函数
来源：http://blog.zdbjq.cn/Article/details/giujpsizb.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.zdbjq.cn/Article/details/gpucldpbs.sHtML

[R30] 函数返回状态码
来源：http://m.share.fehbvm.com/Article/details/ggljaafto.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.fehbvm.com/Article/details/gbqhinnub.sHtML

[R31] 局部变量
来源：http://www.m.share.hesvh.cn/Article/details/gtyhxsbyy.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.zdbjq.cn/Article/details/gyqifhgqd.sHtML

[R32] 参数个数校验
来源：http://www.share.fehbvm.com/Article/details/gcaebpmqn.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.fehbvm.com/Article/details/gfpulckhk.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.zdbjq.cn/Article/details/gpenqnxyf.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.hesvh.cn/Article/details/gvgxavjuf.sHtML

[R34] 退出时清理
来源：http://3g.fehbvm.com/Article/details/gligfbsko.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.zdbjq.cn/Article/details/gqzaxqlkd.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.zdbjq.cn/Article/details/gfsbgpgnl.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.zdbjq.cn/Article/details/gfjpkwkcn.sHtML

[R36] 并发执行多个任务
来源：http://m.share.hesvh.cn/Article/details/ggmfuadpr.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fehbvm.com/Article/details/gkaenchwz.sHtML

[R37] 把输出赋给变量
来源：http://blog.fehbvm.com/Article/details/gyibfloln.sHtML

files=$(ls -1)
来源：http://www.blog.zdbjq.cn/Article/details/gacnyfjbp.sHtML

[R38] 管道串联
来源：http://blog.fehbvm.com/Article/details/geewnsqlc.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.fehbvm.com/Article/details/gjocejwzf.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.zdbjq.cn/Article/details/gmxuykboe.sHtML

cmd > out.log 2>&1
来源：http://www.share.fehbvm.com/Article/details/gocoomlse.sHtML

[R40] 追加写日志
来源：http://www.m.share.hesvh.cn/Article/details/gtomdizjg.sHtML

echo "log" >> out.log
来源：http://www.share.fehbvm.com/Article/details/gfuqrymoi.sHtML

[R41] 丢弃输出
来源：http://mobile.fehbvm.com/Article/details/gncobqxgj.sHtML

cmd >/dev/null 2>&1
来源：http://wap.hesvh.cn/Article/details/gdbkfbwfr.sHtML

[R42] 输入重定向
来源：http://3g.fehbvm.com/Article/details/gaosdwdln.sHtML

wc -l < a.txt
来源：http://mobile.fehbvm.com/Article/details/gyhpiylod.sHtML

[R43] 按名字查找文件
来源：http://blog.hesvh.cn/Article/details/gcxmnyjpp.sHtML

find . -name "*.log" -type f
来源：http://www.blog.zdbjq.cn/Article/details/gmnsosxec.sHtML

[R44] 按修改时间查找
来源：http://wap.fehbvm.com/Article/details/gjfmzvruw.sHtML

find . -mtime -7 -type f
来源：http://www.share.fehbvm.com/Article/details/gzbdbmtqr.sHtML

[R45] 批量删除
来源：http://www.share.fehbvm.com/Article/details/gdpicxbmg.sHtML

find . -name "*.tmp" -delete
来源：http://blog.hesvh.cn/Article/details/ggogcbrau.sHtML

[R46] 递归替换文件内容
来源：http://baike.fehbvm.com/Article/details/gmepjophn.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.zdbjq.cn/Article/details/gyvhyiywu.sHtML

[R47] sed 单行替换
来源：http://www.share.fehbvm.com/Article/details/gnfmrwwea.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.hesvh.cn/Article/details/gdmdeqado.sHtML

[R48] awk 取指定列
来源：http://www.share.zdbjq.cn/Article/details/gtsumfcqq.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.hesvh.cn/Article/details/gpjztxncw.sHtML

[R49] awk 带条件
来源：http://3g.hesvh.cn/Article/details/gxopbbocm.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.zdbjq.cn/Article/details/gumwmyhmu.sHtML

[R50] awk 求和
来源：http://www.blog.zdbjq.cn/Article/details/gwpayirwx.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fehbvm.com/Article/details/gvykdtrgz.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.zdbjq.cn/Article/details/gwwdwcohq.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.fehbvm.com/Article/details/gbhiarfph.sHtML

[R52] 统计行数
来源：http://3g.hesvh.cn/Article/details/gbuyvozsp.sHtML

wc -l a.txt
来源：http://baike.zdbjq.cn/Article/details/gvnsyujbn.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.hesvh.cn/Article/details/gkmgmhgvc.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fehbvm.com/Article/details/gtvmkghwi.sHtML

[R54] 比较两个文件
来源：http://read.share.hesvh.cn/Article/details/gbhqoxobc.sHtML

diff a.txt b.txt
来源：http://www.blog.zdbjq.cn/Article/details/gvlhvwjlw.sHtML

[R55] 压缩与解压
来源：http://wap.zdbjq.cn/Article/details/gwezdrndr.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.zdbjq.cn/Article/details/ggmdkliix.sHtML

[R56] 远程拷贝
来源：http://www.blog.hesvh.cn/Article/details/gtcrmeraa.sHtML

scp file user@host:/path/
来源：http://m.share.fehbvm.com/Article/details/gqhlmavvo.sHtML

[R57] 远程执行命令
来源：http://www.share.fehbvm.com/Article/details/gkajxqvbt.sHtML

ssh user@host 'uptime'
来源：http://3g.zdbjq.cn/Article/details/gbsxqxxve.sHtML

[R58] 下载文件
来源：http://www.m.share.hesvh.cn/Article/details/gmfgjddoz.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.hesvh.cn/Article/details/gpcdycbhv.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.fehbvm.com/Article/details/gotoopdhl.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fehbvm.com/Article/details/glmxyjctx.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.fehbvm.com/Article/details/gcrhraeal.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fehbvm.com/Article/details/glslulrys.sHtML

[R61] 磁盘占用
来源：http://m.share.hesvh.cn/Article/details/gbjfiqqks.sHtML

df -h;  du -sh *
来源：http://www.blog.fehbvm.com/Article/details/gbguiyjux.sHtML

[R62] 找最占空间的文件
来源：http://baike.fehbvm.com/Article/details/gzmvyaamu.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.hesvh.cn/Article/details/gqlligkox.sHtML

[R63] 内存与进程
来源：http://wap.zdbjq.cn/Article/details/gyerufasx.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.zdbjq.cn/Article/details/ghyytfagf.sHtML

[R64] 结束进程
来源：http://www.m.share.hesvh.cn/Article/details/gxodgtltn.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.zdbjq.cn/Article/details/gaenogpby.sHtML

[R65] 查看端口占用
来源：http://blog.fehbvm.com/Article/details/gqgmhvaiu.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.zdbjq.cn/Article/details/ghzdzcigj.sHtML

[R66] 定时任务
来源：http://wap.fehbvm.com/Article/details/gagqbvlfh.sHtML

crontab -e;  crontab -l
来源：http://3g.fehbvm.com/Article/details/gunmcthga.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fehbvm.com/Article/details/gnoqzwirs.sHtML

openssl rand -hex 16
来源：http://wap.fehbvm.com/Article/details/gywqtnsrf.sHtML

[R68] 计算文件校验值
来源：http://wap.fehbvm.com/Article/details/guypcemhq.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.fehbvm.com/Article/details/gvkwjrefu.sHtML

[R69] 生成随机密码
来源：http://mobile.fehbvm.com/Article/details/glhfglzjm.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fehbvm.com/Article/details/gwafsbbxo.sHtML

[R70] 时间戳与互转
来源：http://m.share.zdbjq.cn/Article/details/gkohcyfhk.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.hesvh.cn/Article/details/gyqieveyh.sHtML

[R71] 日期格式化
来源：http://www.m.share.hesvh.cn/Article/details/gyecohcib.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.fehbvm.com/Article/details/gofnrlglc.sHtML

[R72] 等待端口就绪
来源：http://baike.fehbvm.com/Article/details/gjtpsmdik.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.hesvh.cn/Article/details/gxxidjhvk.sHtML

[R73] 分割大日志
来源：http://wap.hesvh.cn/Article/details/gcyipdaak.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.zdbjq.cn/Article/details/gxxzurwdc.sHtML

[R74] 批量重命名
来源：http://www.share.fehbvm.com/Article/details/grgjelipp.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gleqttodb.sHtML

[R75] 导出环境变量
来源：http://read.share.hesvh.cn/Article/details/gzhhfelzz.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.hesvh.cn/Article/details/gitqmhdvf.sHtML

[R76] 使用临时文件
来源：http://m.share.zdbjq.cn/Article/details/gsbgmdsvt.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.hesvh.cn/Article/details/geurqzjgv.sHtML

[R77] 读取用户输入
来源：http://wap.hesvh.cn/Article/details/gqikuhsyq.sHtML

read -rp "请输入: " ans
来源：http://wap.fehbvm.com/Article/details/gealoobuo.sHtML

[R78] 交互式菜单
来源：http://mobile.fehbvm.com/Article/details/gjewuifrr.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.zdbjq.cn/Article/details/gdeupmrhn.sHtML

[R79] 解析命令行选项
来源：http://baike.hesvh.cn/Article/details/ggswzfseb.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.hesvh.cn/Article/details/gvtqqpzjp.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.zdbjq.cn/Article/details/gfychmvon.sHtML

time ./run.sh
来源：http://baike.hesvh.cn/Article/details/gdrltgogj.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gnxixgmos.sHtML

S. C / C++ 专题
来源：http://3g.hesvh.cn/Article/details/ggqgkxtds.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/guomtysrc.sHtML

[S01] C：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gqzhnpzeq.sHtML

#include <stdio.h>
来源：http://3g.fehbvm.com/Article/details/gzploxerb.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fehbvm.com/Article/details/gmoznjkhf.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.zdbjq.cn/Article/details/ghaebqdlh.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fehbvm.com/Article/details/gzeehqfit.sHtML

[S03] C：读入整数
来源：http://wap.fehbvm.com/Article/details/gzjaahpdd.sHtML

int x; scanf("%d", &x);
来源：http://m.share.hesvh.cn/Article/details/gcsacsakr.sHtML

[S04] C：字符串复制
来源：http://read.share.zdbjq.cn/Article/details/guvwxamyz.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.zdbjq.cn/Article/details/glnmhjtcn.sHtML

[S05] C：字符串长度
来源：http://3g.fehbvm.com/Article/details/gzqeudvwg.sHtML

strlen(s)
来源：http://wap.fehbvm.com/Article/details/gbipwraau.sHtML

[S06] C：字符串比较
来源：http://m.share.fehbvm.com/Article/details/gjsesnusz.sHtML

strcmp(a, b) == 0
来源：http://read.share.zdbjq.cn/Article/details/ghdkaqewf.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.zdbjq.cn/Article/details/gvinkporu.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.zdbjq.cn/Article/details/gumrwypek.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fehbvm.com/Article/details/gcpdyyrbb.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fehbvm.com/Article/details/gublzqjdh.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.hesvh.cn/Article/details/gslyqivwk.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.zdbjq.cn/Article/details/gashghhdb.sHtML

[S10] C：指针与解引用
来源：http://mobile.fehbvm.com/Article/details/gyvyzgept.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fehbvm.com/Article/details/gqzvtygiz.sHtML

[S11] C：逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gipytazpn.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.hesvh.cn/Article/details/gnffpjkof.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.zdbjq.cn/Article/details/glaiihejg.sHtML

fclose(f);
来源：http://3g.hesvh.cn/Article/details/gtnecmvyt.sHtML

[S12] C：写文件
来源：http://baike.hesvh.cn/Article/details/ghbshombe.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.zdbjq.cn/Article/details/geuxpznlf.sHtML

[S13] C：宏定义
来源：http://www.share.fehbvm.com/Article/details/gvbplqyup.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.hesvh.cn/Article/details/gevnyryhu.sHtML

[S14] C：枚举
来源：http://3g.zdbjq.cn/Article/details/graiilaan.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.fehbvm.com/Article/details/ghxqrixjj.sHtML

[S15] C：类型转换
来源：http://www.m.share.hesvh.cn/Article/details/gzmeoojlz.sHtML

(double) a / b
来源：http://baike.hesvh.cn/Article/details/gyfojgaoi.sHtML

[S16] C：位操作置位
来源：http://blog.fehbvm.com/Article/details/gvfwcegiu.sHtML

x |= (1 << 3);
来源：http://3g.fehbvm.com/Article/details/gccoisahi.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gqpvssdnu.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.zdbjq.cn/Article/details/grjunrhip.sHtML

[S18] C：命令行参数
来源：http://read.share.hesvh.cn/Article/details/gdmynbkbc.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.zdbjq.cn/Article/details/gaiqrbrlt.sHtML

[S19] C：快速排序
来源：http://blog.hesvh.cn/Article/details/grqmtxwsh.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fehbvm.com/Article/details/gfaqqzbfo.sHtML

[S20] C：二分查找
来源：http://blog.hesvh.cn/Article/details/gnohryepo.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fehbvm.com/Article/details/gmokhwxad.sHtML

[S21] C：字符类别判断
来源：http://mobile.hesvh.cn/Article/details/gtjyboisi.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.hesvh.cn/Article/details/gqlywyzcz.sHtML

[S22] C：字符串转数字
来源：http://mobile.zdbjq.cn/Article/details/gqrxuegry.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.hesvh.cn/Article/details/gpcwnnscq.sHtML

[S23] C：随机数
来源：http://m.share.fehbvm.com/Article/details/gqaygkabk.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.fehbvm.com/Article/details/gzkzwgtip.sHtML

[S24] C：获取本地时间
来源：http://www.share.zdbjq.cn/Article/details/gzyxfiavn.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.hesvh.cn/Article/details/gmlljthxm.sHtML

[S25] C：内存拷贝
来源：http://3g.fehbvm.com/Article/details/gortpofpw.sHtML

memcpy(dst, src, n);
来源：http://baike.zdbjq.cn/Article/details/gqxmweggj.sHtML

[S26] C：内存清零
来源：http://www.share.hesvh.cn/Article/details/gokhecqry.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fehbvm.com/Article/details/gdzztbvfu.sHtML

[S27] C：定义常量
来源：http://wap.zdbjq.cn/Article/details/glgamrurn.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gkityafda.sHtML

[S28] C：静态变量
来源：http://baike.hesvh.cn/Article/details/guasrjqkz.sHtML

static int counter = 0;
来源：http://read.share.zdbjq.cn/Article/details/gbakabsvy.sHtML

[S29] C：变参函数
来源：http://www.blog.fehbvm.com/Article/details/grlhvnmka.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fehbvm.com/Article/details/guwnjgipw.sHtML

[S30] C：头文件保护
来源：http://m.share.zdbjq.cn/Article/details/geyitkfva.sHtML

#ifndef X_H
来源：http://3g.zdbjq.cn/Article/details/gjfqpsuhi.sHtML

#define X_H
来源：http://wap.fehbvm.com/Article/details/gotdpbzis.sHtML

#endif
来源：http://www.blog.fehbvm.com/Article/details/gkwhqnqsi.sHtML

[S31] C++：Hello World
来源：http://3g.fehbvm.com/Article/details/gvmrmsshc.sHtML

#include <iostream>
来源：http://www.m.share.hesvh.cn/Article/details/gvmpndpil.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.zdbjq.cn/Article/details/gcfmjbmxm.sHtML

[S32] C++：字符串
来源：http://m.share.zdbjq.cn/Article/details/gistkulad.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.zdbjq.cn/Article/details/gfdoqhfah.sHtML

[S33] C++：vector 增删
来源：http://m.share.hesvh.cn/Article/details/gsdpnznth.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.zdbjq.cn/Article/details/gjusvjgqm.sHtML

[S34] C++：遍历 vector
来源：http://wap.hesvh.cn/Article/details/gsxhfizwp.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.zdbjq.cn/Article/details/gddtcbpmr.sHtML

[S35] C++：map
来源：http://wap.zdbjq.cn/Article/details/gcgimwnss.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gbliwxugv.sHtML

[S36] C++：unordered_map
来源：http://read.share.hesvh.cn/Article/details/gapckjbtn.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fehbvm.com/Article/details/ggjfivlkc.sHtML

[S37] C++：set
来源：http://read.share.hesvh.cn/Article/details/gotzwfwkx.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.fehbvm.com/Article/details/gqjxbozjf.sHtML

[S38] C++：排序
来源：http://www.share.zdbjq.cn/Article/details/ghksiguys.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.zdbjq.cn/Article/details/gexlphsdq.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.hesvh.cn/Article/details/gifjrpmrv.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.fehbvm.com/Article/details/gnoofrhxx.sHtML

[S40] C++：查找元素
来源：http://wap.hesvh.cn/Article/details/ggjyfcdfr.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.hesvh.cn/Article/details/gpkbznkhs.sHtML

[S41] C++：类与构造函数
来源：http://mobile.fehbvm.com/Article/details/giwragwqv.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.zdbjq.cn/Article/details/gpxvqpooc.sHtML

[S42] C++：继承与虚函数
来源：http://blog.zdbjq.cn/Article/details/gynkupgyc.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fehbvm.com/Article/details/gcvgbkwyv.sHtML

[S43] C++：智能指针
来源：http://3g.zdbjq.cn/Article/details/gfztaapco.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.zdbjq.cn/Article/details/gzwiaxsxx.sHtML

[S44] C++：引用传参
来源：http://mobile.zdbjq.cn/Article/details/gpezwxumi.sHtML

void inc(int &x) { ++x; }
来源：http://blog.zdbjq.cn/Article/details/gehbtkwln.sHtML

[S45] C++：lambda
来源：http://3g.zdbjq.cn/Article/details/gtdpopmox.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.zdbjq.cn/Article/details/gojqvmscc.sHtML

[S46] C++：函数模板
来源：http://blog.zdbjq.cn/Article/details/gojxedbjy.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.zdbjq.cn/Article/details/gtnzwxwln.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.zdbjq.cn/Article/details/giazdtucu.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.hesvh.cn/Article/details/gldcxylta.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gnudwplyz.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.hesvh.cn/Article/details/gwhpmbfeb.sHtML

while (std::getline(in, line)) { }
来源：http://3g.fehbvm.com/Article/details/gmcemvign.sHtML

[S49] C++：写文件
来源：http://www.m.share.fehbvm.com/Article/details/gjpodosjn.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.zdbjq.cn/Article/details/gqsjzcdtz.sHtML

[S50] C++：格式化数字
来源：http://www.share.fehbvm.com/Article/details/gfygcarta.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gjusvcomx.sHtML

[S51] C++：显式类型转换
来源：http://baike.zdbjq.cn/Article/details/gilervlib.sHtML

static_cast<double>(a) / b
来源：http://www.share.fehbvm.com/Article/details/gcblsayjq.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.zdbjq.cn/Article/details/gbqubmobq.sHtML

int size() const noexcept { return n_; }
来源：http://wap.hesvh.cn/Article/details/ghakqxobe.sHtML

[S53] C++：移动语义
来源：http://3g.hesvh.cn/Article/details/gcexymseu.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.zdbjq.cn/Article/details/gfnbpzsnr.sHtML

[S54] C++：异常处理
来源：http://www.blog.fehbvm.com/Article/details/gpqohteys.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.zdbjq.cn/Article/details/gdzmsuuap.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fehbvm.com/Article/details/gqnwoajrm.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.hesvh.cn/Article/details/gqwljcgkb.sHtML

[S56] C++：optional
来源：http://www.m.share.hesvh.cn/Article/details/gaczhdxlw.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.fehbvm.com/Article/details/gmqdlvcws.sHtML

[S57] C++：编译期常量
来源：http://baike.fehbvm.com/Article/details/guaykmvkp.sHtML

constexpr int N = 10;
来源：http://www.share.hesvh.cn/Article/details/gtvrfddum.sHtML

[S58] C++：命名空间
来源：http://www.share.zdbjq.cn/Article/details/gqxhjkrnu.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.hesvh.cn/Article/details/gctjbpawq.sHtML

[S59] C++：静态断言
来源：http://blog.fehbvm.com/Article/details/gxtlweidy.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.hesvh.cn/Article/details/gwgquklmb.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.hesvh.cn/Article/details/gtrargawi.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.zdbjq.cn/Article/details/gqyhivgsj.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gjlaydcod.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fehbvm.com/Article/details/gjfkdicia.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gyrmqubmi.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.fehbvm.com/Article/details/gjahealvv.sHtML

println("Hello")
来源：http://blog.fehbvm.com/Article/details/ghrlqukbg.sHtML

[T02] Kotlin：变量
来源：http://www.blog.zdbjq.cn/Article/details/gcihtfphl.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.zdbjq.cn/Article/details/gyimkzjey.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.zdbjq.cn/Article/details/guvicdowm.sHtML

"值: $b"
来源：http://baike.fehbvm.com/Article/details/gmmvbzsay.sHtML

[T04] Kotlin：空安全
来源：http://wap.fehbvm.com/Article/details/gvxrqhdin.sHtML

val n: String? = null;  n?.length
来源：http://read.share.zdbjq.cn/Article/details/gnrvxynxh.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.fehbvm.com/Article/details/gdtotontn.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.hesvh.cn/Article/details/gwlettujh.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.fehbvm.com/Article/details/giitekxob.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.zdbjq.cn/Article/details/gxraoxqni.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.hesvh.cn/Article/details/gpzktqdcl.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.zdbjq.cn/Article/details/gxvmhszbf.sHtML

[T08] Kotlin：数据类
来源：http://m.share.zdbjq.cn/Article/details/gbpboseot.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.zdbjq.cn/Article/details/gpdywdhni.sHtML


<!-- 参考信息 -->