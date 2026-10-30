代发 wailian999

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.zdbjq.cn/Article/details/gmntnphob.sHtML

[R16] until 等待条件
来源：http://www.m.share.fehbvm.com/Article/details/gsnytacpl.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.hesvh.cn/Article/details/gpohljayb.sHtML

[R17] 数组定义与取值
来源：http://mobile.fehbvm.com/Article/details/gmbcklnfa.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.zdbjq.cn/Article/details/gkjvmxlyw.sHtML

[R18] 遍历数组
来源：http://mobile.hesvh.cn/Article/details/gkitasubf.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.hesvh.cn/Article/details/gazlehwql.sHtML

[R19] 数组长度
来源：http://blog.hesvh.cn/Article/details/gzqyaxcge.sHtML

echo "${#arr[@]}"
来源：http://mobile.zdbjq.cn/Article/details/ghtgxaxpt.sHtML

[R20] 关联数组（字典）
来源：http://read.share.zdbjq.cn/Article/details/gitsgnssa.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.fehbvm.com/Article/details/gukfbqane.sHtML

[R21] 字符串长度
来源：http://wap.hesvh.cn/Article/details/gecxglqby.sHtML

echo "${#s}"
来源：http://baike.hesvh.cn/Article/details/gxybraemv.sHtML

[R22] 截取子串
来源：http://www.m.share.zdbjq.cn/Article/details/gczznapkp.sHtML

echo "${s:0:5}"
来源：http://read.share.hesvh.cn/Article/details/gzavclddm.sHtML

[R23] 字符串替换
来源：http://3g.zdbjq.cn/Article/details/goggtoiwr.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.zdbjq.cn/Article/details/gktgkylnm.sHtML

[R24] 大小写转换
来源：http://3g.hesvh.cn/Article/details/grutagnra.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.hesvh.cn/Article/details/gecqcobaz.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.hesvh.cn/Article/details/gscgdgjtn.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.hesvh.cn/Article/details/guutdxran.sHtML

[R26] 命令替换
来源：http://m.share.zdbjq.cn/Article/details/gnxjaodxo.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.hesvh.cn/Article/details/gbjhsaczy.sHtML

[R27] 算术展开
来源：http://wap.zdbjq.cn/Article/details/gzphpaits.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.zdbjq.cn/Article/details/gdpixrfzk.sHtML

[R28] 浮点运算
来源：http://blog.hesvh.cn/Article/details/ghpmxlpyt.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.hesvh.cn/Article/details/gusyilreh.sHtML

[R29] 定义函数
来源：http://m.share.fehbvm.com/Article/details/glwdzeahs.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.hesvh.cn/Article/details/guwsypmto.sHtML

[R30] 函数返回状态码
来源：http://wap.zdbjq.cn/Article/details/gtantrhux.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.hesvh.cn/Article/details/gjdlzwemu.sHtML

[R31] 局部变量
来源：http://3g.hesvh.cn/Article/details/ggjrexddw.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.zdbjq.cn/Article/details/gwzutbyfn.sHtML

[R32] 参数个数校验
来源：http://www.share.hesvh.cn/Article/details/gwdkkglly.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.hesvh.cn/Article/details/grudegsjr.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.zdbjq.cn/Article/details/glvubveqs.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.hesvh.cn/Article/details/gobvbmsqm.sHtML

[R34] 退出时清理
来源：http://m.share.fehbvm.com/Article/details/gzwgjisyt.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.fehbvm.com/Article/details/gvwfdfuee.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.hesvh.cn/Article/details/gcfhtvywg.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.zdbjq.cn/Article/details/grqzkudip.sHtML

[R36] 并发执行多个任务
来源：http://blog.zdbjq.cn/Article/details/gogupjtqr.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.zdbjq.cn/Article/details/gzuiyusmd.sHtML

[R37] 把输出赋给变量
来源：http://baike.zdbjq.cn/Article/details/gsmguvdwk.sHtML

files=$(ls -1)
来源：http://read.share.zdbjq.cn/Article/details/gdvsuqwng.sHtML

[R38] 管道串联
来源：http://mobile.hesvh.cn/Article/details/gfabiogwm.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.zdbjq.cn/Article/details/gmjxnjsom.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.zdbjq.cn/Article/details/gnlpngtcj.sHtML

cmd > out.log 2>&1
来源：http://www.share.fehbvm.com/Article/details/gsllwajtw.sHtML

[R40] 追加写日志
来源：http://www.blog.zdbjq.cn/Article/details/glynaplzy.sHtML

echo "log" >> out.log
来源：http://www.blog.hesvh.cn/Article/details/gyxebnnyk.sHtML

[R41] 丢弃输出
来源：http://www.m.share.fehbvm.com/Article/details/gmgqyuwov.sHtML

cmd >/dev/null 2>&1
来源：http://baike.zdbjq.cn/Article/details/gaerdpnnk.sHtML

[R42] 输入重定向
来源：http://3g.hesvh.cn/Article/details/gqbwmotwb.sHtML

wc -l < a.txt
来源：http://mobile.zdbjq.cn/Article/details/gflzfraqu.sHtML

[R43] 按名字查找文件
来源：http://m.share.fehbvm.com/Article/details/ghqadtcqw.sHtML

find . -name "*.log" -type f
来源：http://m.share.hesvh.cn/Article/details/geprceffp.sHtML

[R44] 按修改时间查找
来源：http://blog.zdbjq.cn/Article/details/gfvtyhjas.sHtML

find . -mtime -7 -type f
来源：http://blog.fehbvm.com/Article/details/ggybxaopn.sHtML

[R45] 批量删除
来源：http://mobile.zdbjq.cn/Article/details/gnlqdocve.sHtML

find . -name "*.tmp" -delete
来源：http://3g.zdbjq.cn/Article/details/gchvdqyue.sHtML

[R46] 递归替换文件内容
来源：http://m.share.hesvh.cn/Article/details/gzgxomsgr.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.hesvh.cn/Article/details/gyzlnpsbh.sHtML

[R47] sed 单行替换
来源：http://www.share.hesvh.cn/Article/details/gdhxvogkh.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.hesvh.cn/Article/details/gagugglka.sHtML

[R48] awk 取指定列
来源：http://read.share.fehbvm.com/Article/details/gczakxnuv.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.hesvh.cn/Article/details/guorwyant.sHtML

[R49] awk 带条件
来源：http://read.share.fehbvm.com/Article/details/gsgrnyarx.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.zdbjq.cn/Article/details/gedaghrrw.sHtML

[R50] awk 求和
来源：http://wap.zdbjq.cn/Article/details/gnyofxjpx.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.zdbjq.cn/Article/details/ghqxgjuoo.sHtML

[R51] 排序去重取前几
来源：http://baike.zdbjq.cn/Article/details/geofgwzor.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.hesvh.cn/Article/details/gqqfezxig.sHtML

[R52] 统计行数
来源：http://www.blog.fehbvm.com/Article/details/gtbkxichj.sHtML

wc -l a.txt
来源：http://m.share.zdbjq.cn/Article/details/gdqsnivrl.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.zdbjq.cn/Article/details/gvbesgfvb.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fehbvm.com/Article/details/gubcfurek.sHtML

[R54] 比较两个文件
来源：http://read.share.fehbvm.com/Article/details/gxnorszyk.sHtML

diff a.txt b.txt
来源：http://3g.zdbjq.cn/Article/details/goaueakpa.sHtML

[R55] 压缩与解压
来源：http://mobile.fehbvm.com/Article/details/glpwgwhub.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.zdbjq.cn/Article/details/gmcfhdpmh.sHtML

[R56] 远程拷贝
来源：http://www.share.hesvh.cn/Article/details/gfygvmosg.sHtML

scp file user@host:/path/
来源：http://www.blog.zdbjq.cn/Article/details/gzmonxovv.sHtML

[R57] 远程执行命令
来源：http://www.m.share.zdbjq.cn/Article/details/gazbqpfqn.sHtML

ssh user@host 'uptime'
来源：http://www.share.zdbjq.cn/Article/details/gvfznueja.sHtML

[R58] 下载文件
来源：http://blog.hesvh.cn/Article/details/gyqyqergm.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fehbvm.com/Article/details/grvufttbf.sHtML

[R59] 发 POST JSON
来源：http://wap.hesvh.cn/Article/details/gwaloghzs.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.fehbvm.com/Article/details/gbxwotscc.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.fehbvm.com/Article/details/gpckpijwn.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.hesvh.cn/Article/details/gmdrtneqw.sHtML

[R61] 磁盘占用
来源：http://wap.hesvh.cn/Article/details/gyshqgfwx.sHtML

df -h;  du -sh *
来源：http://read.share.fehbvm.com/Article/details/gkibebbsp.sHtML

[R62] 找最占空间的文件
来源：http://blog.zdbjq.cn/Article/details/gopakdzex.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.zdbjq.cn/Article/details/gdvjtpzaj.sHtML

[R63] 内存与进程
来源：http://wap.hesvh.cn/Article/details/gnohlhtng.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.hesvh.cn/Article/details/gbphbqpeb.sHtML

[R64] 结束进程
来源：http://baike.zdbjq.cn/Article/details/gyeukipgs.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fehbvm.com/Article/details/gcjtakuxj.sHtML

[R65] 查看端口占用
来源：http://blog.fehbvm.com/Article/details/grztfajvx.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.hesvh.cn/Article/details/gtipymzym.sHtML

[R66] 定时任务
来源：http://m.share.fehbvm.com/Article/details/ghtfyqdrl.sHtML

crontab -e;  crontab -l
来源：http://mobile.zdbjq.cn/Article/details/guidkqtwc.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.fehbvm.com/Article/details/gvncrbcof.sHtML

openssl rand -hex 16
来源：http://mobile.zdbjq.cn/Article/details/gorbqpxje.sHtML

[R68] 计算文件校验值
来源：http://blog.hesvh.cn/Article/details/gtponzubd.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.hesvh.cn/Article/details/geaazcjfu.sHtML

[R69] 生成随机密码
来源：http://www.share.hesvh.cn/Article/details/gcnvvbcyg.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.zdbjq.cn/Article/details/giqralowj.sHtML

[R70] 时间戳与互转
来源：http://mobile.hesvh.cn/Article/details/geezcvuyq.sHtML

date +%s;  date -d @1700000000
来源：http://blog.hesvh.cn/Article/details/gbpyneeyj.sHtML

[R71] 日期格式化
来源：http://baike.fehbvm.com/Article/details/guzooptjp.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.fehbvm.com/Article/details/gvcypwhpl.sHtML

[R72] 等待端口就绪
来源：http://baike.hesvh.cn/Article/details/gsmboypdv.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fehbvm.com/Article/details/gsjsrrmsr.sHtML

[R73] 分割大日志
来源：http://wap.hesvh.cn/Article/details/gegkansds.sHtML

split -l 1000 big.log part_
来源：http://baike.fehbvm.com/Article/details/gyyoatafk.sHtML

[R74] 批量重命名
来源：http://mobile.fehbvm.com/Article/details/gcdodclov.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.zdbjq.cn/Article/details/ghjqdhbrr.sHtML

[R75] 导出环境变量
来源：http://3g.fehbvm.com/Article/details/gckepyyen.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fehbvm.com/Article/details/gxgnomnso.sHtML

[R76] 使用临时文件
来源：http://www.share.hesvh.cn/Article/details/guyplldqj.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.hesvh.cn/Article/details/gxucoyage.sHtML

[R77] 读取用户输入
来源：http://wap.fehbvm.com/Article/details/gvudzepeg.sHtML

read -rp "请输入: " ans
来源：http://read.share.fehbvm.com/Article/details/gdogvuzbm.sHtML

[R78] 交互式菜单
来源：http://www.blog.hesvh.cn/Article/details/gjeuxvwbg.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.hesvh.cn/Article/details/gebydgvjt.sHtML

[R79] 解析命令行选项
来源：http://m.share.zdbjq.cn/Article/details/guectvknp.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fehbvm.com/Article/details/grbtqteaq.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.fehbvm.com/Article/details/gyzxkddeu.sHtML

time ./run.sh
来源：http://wap.zdbjq.cn/Article/details/gbfsgzhjz.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gcuwluvpi.sHtML

S. C / C++ 专题
来源：http://blog.hesvh.cn/Article/details/gbfzkbrbi.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gyitezpca.sHtML

[S01] C：Hello World
来源：http://www.blog.hesvh.cn/Article/details/glkebzzbc.sHtML

#include <stdio.h>
来源：http://www.blog.fehbvm.com/Article/details/gigpguham.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.zdbjq.cn/Article/details/gsoggzkvd.sHtML

[S02] C：变量与格式化输出
来源：http://blog.zdbjq.cn/Article/details/giomvfvtl.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.hesvh.cn/Article/details/gcgimkrcd.sHtML

[S03] C：读入整数
来源：http://read.share.hesvh.cn/Article/details/gmqucknee.sHtML

int x; scanf("%d", &x);
来源：http://3g.fehbvm.com/Article/details/gatffrpga.sHtML

[S04] C：字符串复制
来源：http://m.share.hesvh.cn/Article/details/gjoawqnkz.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.fehbvm.com/Article/details/grvstkjkx.sHtML

[S05] C：字符串长度
来源：http://m.share.zdbjq.cn/Article/details/gejwipbcp.sHtML

strlen(s)
来源：http://www.blog.fehbvm.com/Article/details/gtskdawfo.sHtML

[S06] C：字符串比较
来源：http://baike.hesvh.cn/Article/details/garxpuvgx.sHtML

strcmp(a, b) == 0
来源：http://baike.zdbjq.cn/Article/details/goupxparw.sHtML

[S07] C：数组遍历求和
来源：http://blog.zdbjq.cn/Article/details/giajgmsgm.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.hesvh.cn/Article/details/gcmrxrqza.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.hesvh.cn/Article/details/gdqrqfsky.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.fehbvm.com/Article/details/gttgjolbu.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.hesvh.cn/Article/details/gpypiizzb.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.fehbvm.com/Article/details/gmthadljr.sHtML

[S10] C：指针与解引用
来源：http://3g.hesvh.cn/Article/details/gzuvdfxzc.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.fehbvm.com/Article/details/grjylgqsp.sHtML

[S11] C：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gnnulqmwd.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.hesvh.cn/Article/details/gkuxmlgjb.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.zdbjq.cn/Article/details/guvunftbs.sHtML

fclose(f);
来源：http://www.share.hesvh.cn/Article/details/gsdtvhuke.sHtML

[S12] C：写文件
来源：http://m.share.hesvh.cn/Article/details/guxbvzdkn.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.zdbjq.cn/Article/details/gtlskptbv.sHtML

[S13] C：宏定义
来源：http://blog.hesvh.cn/Article/details/grxnwxmuv.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.zdbjq.cn/Article/details/gcyznoaif.sHtML

[S14] C：枚举
来源：http://read.share.zdbjq.cn/Article/details/gqcjuuczi.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.zdbjq.cn/Article/details/gmeuenfpw.sHtML

[S15] C：类型转换
来源：http://mobile.zdbjq.cn/Article/details/gfhptrxqc.sHtML

(double) a / b
来源：http://m.share.zdbjq.cn/Article/details/gkdwekdyn.sHtML

[S16] C：位操作置位
来源：http://mobile.fehbvm.com/Article/details/gakiqsktg.sHtML

x |= (1 << 3);
来源：http://blog.fehbvm.com/Article/details/gcanxnayu.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fehbvm.com/Article/details/goysgsabj.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.zdbjq.cn/Article/details/gsntlhngi.sHtML

[S18] C：命令行参数
来源：http://3g.fehbvm.com/Article/details/glxljyfuw.sHtML

int main(int argc, char **argv)
来源：http://m.share.hesvh.cn/Article/details/gqlfojrck.sHtML

[S19] C：快速排序
来源：http://baike.zdbjq.cn/Article/details/gydvchokl.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.zdbjq.cn/Article/details/gkccvgdbh.sHtML

[S20] C：二分查找
来源：http://3g.zdbjq.cn/Article/details/gjhrgkglc.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.hesvh.cn/Article/details/gmmxlnfjx.sHtML

[S21] C：字符类别判断
来源：http://read.share.fehbvm.com/Article/details/gnelsycbj.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.hesvh.cn/Article/details/guvnwcxjz.sHtML

[S22] C：字符串转数字
来源：http://baike.hesvh.cn/Article/details/glyytnuiu.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.hesvh.cn/Article/details/gwypymhml.sHtML

[S23] C：随机数
来源：http://baike.hesvh.cn/Article/details/gcxwspzky.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fehbvm.com/Article/details/gqagdrxtx.sHtML

[S24] C：获取本地时间
来源：http://mobile.zdbjq.cn/Article/details/gvjwvpgvg.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fehbvm.com/Article/details/gshstgacd.sHtML

[S25] C：内存拷贝
来源：http://www.share.hesvh.cn/Article/details/geibngvhw.sHtML

memcpy(dst, src, n);
来源：http://3g.zdbjq.cn/Article/details/gzubzkedv.sHtML

[S26] C：内存清零
来源：http://www.blog.hesvh.cn/Article/details/gbsyinpfg.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.zdbjq.cn/Article/details/gkecyjiwe.sHtML

[S27] C：定义常量
来源：http://mobile.hesvh.cn/Article/details/gtpyxxwry.sHtML

const double PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gbtzkhmao.sHtML

[S28] C：静态变量
来源：http://www.share.zdbjq.cn/Article/details/geciqxxpg.sHtML

static int counter = 0;
来源：http://mobile.zdbjq.cn/Article/details/gexblqsod.sHtML

[S29] C：变参函数
来源：http://www.share.fehbvm.com/Article/details/gwkjswsfk.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.zdbjq.cn/Article/details/gsflidffc.sHtML

[S30] C：头文件保护
来源：http://mobile.zdbjq.cn/Article/details/gbvhkhjdp.sHtML

#ifndef X_H
来源：http://www.blog.hesvh.cn/Article/details/gskdyqktd.sHtML

#define X_H
来源：http://mobile.zdbjq.cn/Article/details/gqmwbgycz.sHtML

#endif
来源：http://m.share.fehbvm.com/Article/details/gpfcbimqe.sHtML

[S31] C++：Hello World
来源：http://mobile.fehbvm.com/Article/details/gyilskmjw.sHtML

#include <iostream>
来源：http://wap.fehbvm.com/Article/details/ggndwsvkw.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.zdbjq.cn/Article/details/gipfohfic.sHtML

[S32] C++：字符串
来源：http://www.share.zdbjq.cn/Article/details/gqanclkdn.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.hesvh.cn/Article/details/gvpuyuepc.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fehbvm.com/Article/details/gxhetitea.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.fehbvm.com/Article/details/gxzcgbtdq.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.zdbjq.cn/Article/details/gczydpbne.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.hesvh.cn/Article/details/glspcqmtx.sHtML

[S35] C++：map
来源：http://m.share.fehbvm.com/Article/details/gayclcnyk.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fehbvm.com/Article/details/gplxgcbwj.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.hesvh.cn/Article/details/gbjnxokos.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gdimugjsb.sHtML

[S37] C++：set
来源：http://wap.zdbjq.cn/Article/details/gjendiiyk.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.zdbjq.cn/Article/details/gecfahryf.sHtML

[S38] C++：排序
来源：http://3g.hesvh.cn/Article/details/gkkavzvtv.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.fehbvm.com/Article/details/gaavcbrko.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.zdbjq.cn/Article/details/gtziniknk.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.hesvh.cn/Article/details/gfbnguwaw.sHtML

[S40] C++：查找元素
来源：http://www.share.fehbvm.com/Article/details/giztdiniw.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.fehbvm.com/Article/details/grwqedxjx.sHtML

[S41] C++：类与构造函数
来源：http://wap.fehbvm.com/Article/details/gvcqfvaci.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.fehbvm.com/Article/details/gnwddvzvc.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.hesvh.cn/Article/details/glyjbgjcn.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.hesvh.cn/Article/details/guvnskoqt.sHtML

[S43] C++：智能指针
来源：http://www.share.fehbvm.com/Article/details/ghkgkplvi.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fehbvm.com/Article/details/giiarofeo.sHtML

[S44] C++：引用传参
来源：http://www.blog.fehbvm.com/Article/details/gdmkbpxwl.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.hesvh.cn/Article/details/grtxtfaut.sHtML

[S45] C++：lambda
来源：http://read.share.hesvh.cn/Article/details/gdlrqgwzl.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.hesvh.cn/Article/details/ghnltappd.sHtML

[S46] C++：函数模板
来源：http://mobile.hesvh.cn/Article/details/gcbzcddyg.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.hesvh.cn/Article/details/gaijolecd.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.hesvh.cn/Article/details/gdteddgab.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.fehbvm.com/Article/details/gcxdodoyp.sHtML

[S48] C++：逐行读文件
来源：http://blog.hesvh.cn/Article/details/gphhkbetl.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.fehbvm.com/Article/details/grxzturxs.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.hesvh.cn/Article/details/gwdrrlaos.sHtML

[S49] C++：写文件
来源：http://read.share.fehbvm.com/Article/details/gmzzmiqjj.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.fehbvm.com/Article/details/gttjhvkru.sHtML

[S50] C++：格式化数字
来源：http://m.share.fehbvm.com/Article/details/gcqhjqsby.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.fehbvm.com/Article/details/ghuhcqolk.sHtML

[S51] C++：显式类型转换
来源：http://read.share.hesvh.cn/Article/details/gbpoefiqy.sHtML

static_cast<double>(a) / b
来源：http://wap.fehbvm.com/Article/details/gzjbrqwuz.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.hesvh.cn/Article/details/glmgxginl.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.zdbjq.cn/Article/details/gytuixkyy.sHtML

[S53] C++：移动语义
来源：http://m.share.hesvh.cn/Article/details/gmahoyaip.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.fehbvm.com/Article/details/gkrjbnbcn.sHtML

[S54] C++：异常处理
来源：http://www.blog.fehbvm.com/Article/details/gounskcna.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.zdbjq.cn/Article/details/gmhuwmcuj.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.hesvh.cn/Article/details/gcrqgflgt.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.fehbvm.com/Article/details/girlpkepa.sHtML

[S56] C++：optional
来源：http://www.blog.zdbjq.cn/Article/details/gctskobka.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.fehbvm.com/Article/details/glhmwdppm.sHtML

[S57] C++：编译期常量
来源：http://www.blog.zdbjq.cn/Article/details/gkwltiwed.sHtML

constexpr int N = 10;
来源：http://www.blog.fehbvm.com/Article/details/gtherorgo.sHtML

[S58] C++：命名空间
来源：http://www.m.share.zdbjq.cn/Article/details/gblirfzjp.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.hesvh.cn/Article/details/gvnsngnut.sHtML

[S59] C++：静态断言
来源：http://www.m.share.hesvh.cn/Article/details/gjawwxnau.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.hesvh.cn/Article/details/gqgzvtmci.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.zdbjq.cn/Article/details/glgnegiug.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fehbvm.com/Article/details/goecozztz.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gslagyfio.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.hesvh.cn/Article/details/gllsbesww.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gilzegfya.sHtML

[T01] Kotlin：Hello World
来源：http://baike.hesvh.cn/Article/details/glctizgsj.sHtML

println("Hello")
来源：http://wap.zdbjq.cn/Article/details/gbgopsxxd.sHtML

[T02] Kotlin：变量
来源：http://www.share.fehbvm.com/Article/details/grygglerx.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.hesvh.cn/Article/details/gelqgwgev.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.fehbvm.com/Article/details/gqbgllnbe.sHtML

"值: $b"
来源：http://wap.fehbvm.com/Article/details/gycsvhllg.sHtML

[T04] Kotlin：空安全
来源：http://blog.fehbvm.com/Article/details/grpmwmbeg.sHtML

val n: String? = null;  n?.length
来源：http://mobile.hesvh.cn/Article/details/gnakjlanh.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.hesvh.cn/Article/details/gzrcrjkki.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.zdbjq.cn/Article/details/gcfkctjvm.sHtML

[T06] Kotlin：集合映射
来源：http://3g.zdbjq.cn/Article/details/geheengxl.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.fehbvm.com/Article/details/gqioaumwi.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.fehbvm.com/Article/details/gbgtkcisx.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.fehbvm.com/Article/details/gcrjowjap.sHtML

[T08] Kotlin：数据类
来源：http://mobile.hesvh.cn/Article/details/gwsephbwf.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.zdbjq.cn/Article/details/gcvtxcmbf.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.fehbvm.com/Article/details/giqsizbfv.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.zdbjq.cn/Article/details/glwxdiuax.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.zdbjq.cn/Article/details/gwnhypodm.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.fehbvm.com/Article/details/gsvxfopob.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.fehbvm.com/Article/details/gxyfxagft.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.hesvh.cn/Article/details/gqaxjipds.sHtML

[T12] Kotlin：解构声明
来源：http://blog.fehbvm.com/Article/details/ghckbxktu.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.fehbvm.com/Article/details/gkptimpbo.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.zdbjq.cn/Article/details/gxgqlwybj.sHtML

val m = mapOf("a" to 1)
来源：http://blog.fehbvm.com/Article/details/gxzxeryno.sHtML

[T14] Kotlin：循环
来源：http://mobile.hesvh.cn/Article/details/gvycgaxha.sHtML

for (i in 1..10) println(i)
来源：http://mobile.zdbjq.cn/Article/details/guehegnzy.sHtML

[T15] Kotlin：接口
来源：http://wap.zdbjq.cn/Article/details/gzooxvujn.sHtML

interface Shape { fun area(): Double }
来源：http://wap.fehbvm.com/Article/details/gmhuxnzgx.sHtML

[T16] Swift：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gdngfriym.sHtML

print("Hello")
来源：http://www.share.hesvh.cn/Article/details/gucqtozgt.sHtML

[T17] Swift：变量与常量
来源：http://blog.hesvh.cn/Article/details/gmkpcptiy.sHtML

var a = 1;  let b = 2
来源：http://read.share.hesvh.cn/Article/details/gwvqyjcxv.sHtML

[T18] Swift：字符串插值
来源：http://wap.fehbvm.com/Article/details/gotkxjpvg.sHtML

"值: \(b)"
来源：http://read.share.hesvh.cn/Article/details/glfcxbuqh.sHtML


<!-- 参考信息 -->