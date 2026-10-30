代发 wailian999

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gazoicafw.sHtML

[R24] 大小写转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gvoimrtmm.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjkononsb.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.fanxiaobao.xyz/Article/details/gktagxifw.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/glkqknpwd.sHtML

[R26] 命令替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gishmajom.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.fanxiaobao.xyz/Article/details/guejhmjrl.sHtML

[R27] 算术展开
来源：http://3g.fanxiaobao.xyz/Article/details/gsxbkwocu.sHtML

echo $((1 + 2 * 3))
来源：http://3g.fanxiaobao.xyz/Article/details/galszytpl.sHtML

[R28] 浮点运算
来源：http://m.share.fanxiaobao.xyz/Article/details/goeguzgsj.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghzyaeshe.sHtML

[R29] 定义函数
来源：http://3g.fanxiaobao.xyz/Article/details/gmgwqvcmh.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fanxiaobao.xyz/Article/details/gbmdqlcqt.sHtML

[R30] 函数返回状态码
来源：http://read.share.fanxiaobao.xyz/Article/details/gsioklzvg.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.fanxiaobao.xyz/Article/details/glhxkccwk.sHtML

[R31] 局部变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gcgvlyxtn.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gdqfjbbqr.sHtML

[R32] 参数个数校验
来源：http://www.share.fanxiaobao.xyz/Article/details/gjotmutas.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gzlqztdav.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjnpfuhdz.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.fanxiaobao.xyz/Article/details/gwlorakxk.sHtML

[R34] 退出时清理
来源：http://mobile.fanxiaobao.xyz/Article/details/ghsfpfdfs.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxrktrfmi.sHtML

[R35] 后台执行并等待
来源：http://blog.fanxiaobao.xyz/Article/details/gjfnspqdy.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gytlxluqw.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gtvcqwwxl.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.fanxiaobao.xyz/Article/details/geulqtkzc.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gztalhjju.sHtML

files=$(ls -1)
来源：http://read.share.fanxiaobao.xyz/Article/details/glifftrpi.sHtML

[R38] 管道串联
来源：http://blog.fanxiaobao.xyz/Article/details/gpmtmfzta.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guszxosde.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmmcxmapy.sHtML

cmd > out.log 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/goabvhnci.sHtML

[R40] 追加写日志
来源：http://wap.fanxiaobao.xyz/Article/details/gjbtwflph.sHtML

echo "log" >> out.log
来源：http://read.share.fanxiaobao.xyz/Article/details/gdusdobkh.sHtML

[R41] 丢弃输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gvrxetuua.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grndzzhtp.sHtML

[R42] 输入重定向
来源：http://wap.fanxiaobao.xyz/Article/details/grurvsllj.sHtML

wc -l < a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/glxxyosom.sHtML

[R43] 按名字查找文件
来源：http://3g.fanxiaobao.xyz/Article/details/geyeypfsd.sHtML

find . -name "*.log" -type f
来源：http://3g.fanxiaobao.xyz/Article/details/gywrbvywr.sHtML

[R44] 按修改时间查找
来源：http://3g.fanxiaobao.xyz/Article/details/gtcyhiloh.sHtML

find . -mtime -7 -type f
来源：http://wap.fanxiaobao.xyz/Article/details/gdlnezlvz.sHtML

[R45] 批量删除
来源：http://www.share.fanxiaobao.xyz/Article/details/gyrmhqdei.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.fanxiaobao.xyz/Article/details/gwzbexgtu.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghnhzrtml.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.fanxiaobao.xyz/Article/details/gmvpkqhiw.sHtML

[R47] sed 单行替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqtvajrfm.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/ghwcqtysw.sHtML

[R48] awk 取指定列
来源：http://read.share.fanxiaobao.xyz/Article/details/gpeubevju.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gwrfciobq.sHtML

[R49] awk 带条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gyllyeaio.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fanxiaobao.xyz/Article/details/gbqmamgsx.sHtML

[R50] awk 求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gkadmyple.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggdbixwyr.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwfvbbrjs.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fanxiaobao.xyz/Article/details/gsuqbeyje.sHtML

[R52] 统计行数
来源：http://m.share.fanxiaobao.xyz/Article/details/gyopvxcmd.sHtML

wc -l a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gnbmxpltj.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqkgnldaf.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.fanxiaobao.xyz/Article/details/gmjuxbbmg.sHtML

[R54] 比较两个文件
来源：http://baike.fanxiaobao.xyz/Article/details/glvmeebqk.sHtML

diff a.txt b.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gxkyflgvc.sHtML

[R55] 压缩与解压
来源：http://www.share.fanxiaobao.xyz/Article/details/ghilwsyqh.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fanxiaobao.xyz/Article/details/gsvnhrbhw.sHtML

[R56] 远程拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/ghudzxcft.sHtML

scp file user@host:/path/
来源：http://wap.fanxiaobao.xyz/Article/details/gjoahpbfw.sHtML

[R57] 远程执行命令
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqhomukwr.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghnuaajik.sHtML

[R58] 下载文件
来源：http://3g.fanxiaobao.xyz/Article/details/gzreuatcv.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.fanxiaobao.xyz/Article/details/gqujklnky.sHtML

[R59] 发 POST JSON
来源：http://www.blog.fanxiaobao.xyz/Article/details/gelkxiqno.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fanxiaobao.xyz/Article/details/gkazzgdar.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/gwlpwyydk.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fanxiaobao.xyz/Article/details/gitkqigxs.sHtML

[R61] 磁盘占用
来源：http://wap.fanxiaobao.xyz/Article/details/geoiwkmvh.sHtML

df -h;  du -sh *
来源：http://read.share.fanxiaobao.xyz/Article/details/gyeyhlwyl.sHtML

[R62] 找最占空间的文件
来源：http://blog.fanxiaobao.xyz/Article/details/gmsnkuntj.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.fanxiaobao.xyz/Article/details/glaefgnov.sHtML

[R63] 内存与进程
来源：http://wap.fanxiaobao.xyz/Article/details/gdyjhjtpf.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.fanxiaobao.xyz/Article/details/gciislgyf.sHtML

[R64] 结束进程
来源：http://blog.fanxiaobao.xyz/Article/details/gdcnbpjac.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.fanxiaobao.xyz/Article/details/glfuarnfa.sHtML

[R65] 查看端口占用
来源：http://baike.fanxiaobao.xyz/Article/details/gtwcseglq.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fanxiaobao.xyz/Article/details/gjuftpiqa.sHtML

[R66] 定时任务
来源：http://m.share.fanxiaobao.xyz/Article/details/geitfxidg.sHtML

crontab -e;  crontab -l
来源：http://read.share.fanxiaobao.xyz/Article/details/gtfjtoozn.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fanxiaobao.xyz/Article/details/gtadsjiec.sHtML

openssl rand -hex 16
来源：http://m.share.fanxiaobao.xyz/Article/details/gdxvfqqax.sHtML

[R68] 计算文件校验值
来源：http://blog.fanxiaobao.xyz/Article/details/gxqgsqvau.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gyfhcmhyj.sHtML

[R69] 生成随机密码
来源：http://wap.fanxiaobao.xyz/Article/details/gscsnvpuy.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gatlkamqa.sHtML

[R70] 时间戳与互转
来源：http://read.share.fanxiaobao.xyz/Article/details/gythgzbff.sHtML

date +%s;  date -d @1700000000
来源：http://baike.fanxiaobao.xyz/Article/details/ggviicuwa.sHtML

[R71] 日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gjeequcab.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.fanxiaobao.xyz/Article/details/gvzshmtuy.sHtML

[R72] 等待端口就绪
来源：http://3g.fanxiaobao.xyz/Article/details/gpahcrhqi.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fanxiaobao.xyz/Article/details/grdbxybzp.sHtML

[R73] 分割大日志
来源：http://wap.fanxiaobao.xyz/Article/details/gfojvsilr.sHtML

split -l 1000 big.log part_
来源：http://baike.fanxiaobao.xyz/Article/details/ggqfztumq.sHtML

[R74] 批量重命名
来源：http://www.m.share.fanxiaobao.xyz/Article/details/genrtlrqr.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gxxdhrnnh.sHtML

[R75] 导出环境变量
来源：http://www.share.fanxiaobao.xyz/Article/details/guctdvhyy.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fanxiaobao.xyz/Article/details/gfvbnccbs.sHtML

[R76] 使用临时文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gwybdnctl.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/gweudirpf.sHtML

[R77] 读取用户输入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnrrsmrak.sHtML

read -rp "请输入: " ans
来源：http://mobile.fanxiaobao.xyz/Article/details/gxzshtkic.sHtML

[R78] 交互式菜单
来源：http://wap.fanxiaobao.xyz/Article/details/giqiwibwg.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpcfmjzde.sHtML

[R79] 解析命令行选项
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbvgfocxp.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fanxiaobao.xyz/Article/details/giuvijbaz.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fanxiaobao.xyz/Article/details/gyhvodqll.sHtML

time ./run.sh
来源：http://baike.fanxiaobao.xyz/Article/details/gvjbrfkjw.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/giymfkmxw.sHtML

S. C / C++ 专题
来源：http://baike.fanxiaobao.xyz/Article/details/gywzdigdv.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gwvhcawzw.sHtML

[S01] C：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gmzxmpwux.sHtML

#include <stdio.h>
来源：http://baike.fanxiaobao.xyz/Article/details/gqtejrfng.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fanxiaobao.xyz/Article/details/ghposfamh.sHtML

[S02] C：变量与格式化输出
来源：http://blog.fanxiaobao.xyz/Article/details/gnpgybtjk.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fanxiaobao.xyz/Article/details/ggeonmjvx.sHtML

[S03] C：读入整数
来源：http://3g.fanxiaobao.xyz/Article/details/gjoecizri.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcbioqgpy.sHtML

[S04] C：字符串复制
来源：http://3g.fanxiaobao.xyz/Article/details/ggwzamnzd.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.fanxiaobao.xyz/Article/details/gwletuved.sHtML

[S05] C：字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcxbdqtfn.sHtML

strlen(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gugugcnkc.sHtML

[S06] C：字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxtataubx.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzmlejkmp.sHtML

[S07] C：数组遍历求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gaimbnrvq.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fanxiaobao.xyz/Article/details/gigoywflq.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fanxiaobao.xyz/Article/details/ggikhewki.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.fanxiaobao.xyz/Article/details/giutunixm.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fanxiaobao.xyz/Article/details/geepabluu.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.fanxiaobao.xyz/Article/details/gjcxttzse.sHtML

[S10] C：指针与解引用
来源：http://wap.fanxiaobao.xyz/Article/details/gcsjkfcho.sHtML

int *p = &a;  *p = 5;
来源：http://3g.fanxiaobao.xyz/Article/details/grgmxixmp.sHtML

[S11] C：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/ggatdlemw.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.fanxiaobao.xyz/Article/details/gilkyfxtu.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gwgyxsmrh.sHtML

fclose(f);
来源：http://mobile.fanxiaobao.xyz/Article/details/goytazjql.sHtML

[S12] C：写文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gbgznuwqk.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.fanxiaobao.xyz/Article/details/gbfugtjbw.sHtML

[S13] C：宏定义
来源：http://www.share.fanxiaobao.xyz/Article/details/grtyebwql.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.fanxiaobao.xyz/Article/details/gvwntqzxx.sHtML

[S14] C：枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/gwdjnpotc.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.fanxiaobao.xyz/Article/details/gcjytfqqn.sHtML

[S15] C：类型转换
来源：http://wap.fanxiaobao.xyz/Article/details/gkubdwqxi.sHtML

(double) a / b
来源：http://3g.fanxiaobao.xyz/Article/details/gcgiojdon.sHtML

[S16] C：位操作置位
来源：http://read.share.fanxiaobao.xyz/Article/details/gtovnkhxk.sHtML

x |= (1 << 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gmwbkyrwd.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcrzbumnd.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.fanxiaobao.xyz/Article/details/ghflioosp.sHtML

[S18] C：命令行参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gcpjgbwel.sHtML

int main(int argc, char **argv)
来源：http://3g.fanxiaobao.xyz/Article/details/gtqfhithj.sHtML

[S19] C：快速排序
来源：http://blog.fanxiaobao.xyz/Article/details/giqfnfyew.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjvqoxfso.sHtML

[S20] C：二分查找
来源：http://wap.fanxiaobao.xyz/Article/details/ghtjnrcfj.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqucsxxdc.sHtML

[S21] C：字符类别判断
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmjhwrbgg.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.fanxiaobao.xyz/Article/details/gufwhnudv.sHtML

[S22] C：字符串转数字
来源：http://mobile.fanxiaobao.xyz/Article/details/grgkjrkgf.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fanxiaobao.xyz/Article/details/gsxpliesa.sHtML

[S23] C：随机数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtivdrhjk.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.fanxiaobao.xyz/Article/details/gasgoewtb.sHtML

[S24] C：获取本地时间
来源：http://wap.fanxiaobao.xyz/Article/details/gpakbxxcf.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghsfveraf.sHtML

[S25] C：内存拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gypqxulli.sHtML

memcpy(dst, src, n);
来源：http://www.share.fanxiaobao.xyz/Article/details/gmwsegzyz.sHtML

[S26] C：内存清零
来源：http://3g.fanxiaobao.xyz/Article/details/gopmeenlk.sHtML

memset(a, 0, sizeof a);
来源：http://baike.fanxiaobao.xyz/Article/details/gtktwwhpj.sHtML

[S27] C：定义常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtwidaiau.sHtML

const double PI = 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/griyrdtca.sHtML

[S28] C：静态变量
来源：http://blog.fanxiaobao.xyz/Article/details/ghkqnphlx.sHtML

static int counter = 0;
来源：http://mobile.fanxiaobao.xyz/Article/details/gnahvxbfy.sHtML

[S29] C：变参函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gmjldmhgy.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fanxiaobao.xyz/Article/details/gnkmipspb.sHtML

[S30] C：头文件保护
来源：http://wap.fanxiaobao.xyz/Article/details/guagbzxge.sHtML

#ifndef X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/ggfjfclgc.sHtML

#define X_H
来源：http://wap.fanxiaobao.xyz/Article/details/ggzbhrxcg.sHtML

#endif
来源：http://mobile.fanxiaobao.xyz/Article/details/gnlajhpyl.sHtML

[S31] C++：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/geltqtkes.sHtML

#include <iostream>
来源：http://wap.fanxiaobao.xyz/Article/details/gjcktgvux.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gwitwcvsm.sHtML

[S32] C++：字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gztkjttwu.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsrrytzfl.sHtML

[S33] C++：vector 增删
来源：http://wap.fanxiaobao.xyz/Article/details/gprcjrynj.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.fanxiaobao.xyz/Article/details/guwuegidx.sHtML

[S34] C++：遍历 vector
来源：http://www.share.fanxiaobao.xyz/Article/details/gfrrnsngz.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gtfhxrswr.sHtML

[S35] C++：map
来源：http://wap.fanxiaobao.xyz/Article/details/gkxecugyr.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gseuhdmaa.sHtML

[S36] C++：unordered_map
来源：http://wap.fanxiaobao.xyz/Article/details/gkfxhhpdz.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gauifidnp.sHtML

[S37] C++：set
来源：http://www.share.fanxiaobao.xyz/Article/details/gaijrpjkv.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/guwheuncy.sHtML

[S38] C++：排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gngqqjcux.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/gmgktqijk.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.fanxiaobao.xyz/Article/details/gydpjoxnh.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fanxiaobao.xyz/Article/details/gpdtcsncc.sHtML

[S40] C++：查找元素
来源：http://blog.fanxiaobao.xyz/Article/details/glzwyudns.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gagafjdbg.sHtML

[S41] C++：类与构造函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gvjrinwoj.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fanxiaobao.xyz/Article/details/gyisjbzee.sHtML

[S42] C++：继承与虚函数
来源：http://blog.fanxiaobao.xyz/Article/details/gectacdjd.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.fanxiaobao.xyz/Article/details/gjhjmabfl.sHtML

[S43] C++：智能指针
来源：http://3g.fanxiaobao.xyz/Article/details/gwodjlary.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.fanxiaobao.xyz/Article/details/gtvafinot.sHtML

[S44] C++：引用传参
来源：http://m.share.fanxiaobao.xyz/Article/details/gyvvfegoy.sHtML

void inc(int &x) { ++x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gcwrhkrna.sHtML

[S45] C++：lambda
来源：http://baike.fanxiaobao.xyz/Article/details/gcymjsgpd.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.fanxiaobao.xyz/Article/details/gvtzjfijx.sHtML

[S46] C++：函数模板
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdhxklncu.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggwaxaipy.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggzqjrtic.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gxqjnxyvf.sHtML

[S48] C++：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gjebubrcl.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.fanxiaobao.xyz/Article/details/gzifrruwt.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtbuzvyqx.sHtML

[S49] C++：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gdwtgjojq.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.fanxiaobao.xyz/Article/details/gyrnczste.sHtML

[S50] C++：格式化数字
来源：http://3g.fanxiaobao.xyz/Article/details/gqdmhwcxq.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/gzjjeyvaj.sHtML

[S51] C++：显式类型转换
来源：http://wap.fanxiaobao.xyz/Article/details/gsoenlceh.sHtML

static_cast<double>(a) / b
来源：http://baike.fanxiaobao.xyz/Article/details/gkgxlxaui.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.fanxiaobao.xyz/Article/details/gnyqctycp.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdunqramn.sHtML

[S53] C++：移动语义
来源：http://baike.fanxiaobao.xyz/Article/details/gtcwaebmf.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.fanxiaobao.xyz/Article/details/gldbzmjim.sHtML

[S54] C++：异常处理
来源：http://3g.fanxiaobao.xyz/Article/details/gwryvkifh.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gntmzulkf.sHtML

[S55] C++：结构化绑定
来源：http://3g.fanxiaobao.xyz/Article/details/gmllgpwdd.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.fanxiaobao.xyz/Article/details/glwtrcwdn.sHtML

[S56] C++：optional
来源：http://www.share.fanxiaobao.xyz/Article/details/geyedknol.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.fanxiaobao.xyz/Article/details/giozuywxq.sHtML

[S57] C++：编译期常量
来源：http://blog.fanxiaobao.xyz/Article/details/gxntmffwo.sHtML

constexpr int N = 10;
来源：http://wap.fanxiaobao.xyz/Article/details/girpjegzv.sHtML

[S58] C++：命名空间
来源：http://wap.fanxiaobao.xyz/Article/details/gunsdxrxc.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.fanxiaobao.xyz/Article/details/grjykriun.sHtML

[S59] C++：静态断言
来源：http://m.share.fanxiaobao.xyz/Article/details/gjtrfhiqi.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.fanxiaobao.xyz/Article/details/gvqcktwno.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.fanxiaobao.xyz/Article/details/goofjijjz.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.fanxiaobao.xyz/Article/details/gobelwrxi.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gltmskqtf.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwbctlywa.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gyhvxekzr.sHtML

[T01] Kotlin：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gnqkdzrdo.sHtML

println("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gidrwkdrc.sHtML

[T02] Kotlin：变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gdydfozmc.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.fanxiaobao.xyz/Article/details/gdvlxehtc.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.fanxiaobao.xyz/Article/details/gsgzdahdg.sHtML

"值: $b"
来源：http://wap.fanxiaobao.xyz/Article/details/ggipdooyk.sHtML

[T04] Kotlin：空安全
来源：http://wap.fanxiaobao.xyz/Article/details/gtaeufuol.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fanxiaobao.xyz/Article/details/gbtdafscg.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/grojqlwrj.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.fanxiaobao.xyz/Article/details/grlorgvpz.sHtML

[T06] Kotlin：集合映射
来源：http://baike.fanxiaobao.xyz/Article/details/gsijqmanp.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gatmapdpt.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/guiqfcsgp.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.fanxiaobao.xyz/Article/details/goiokkmiu.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glvndedef.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdpcgxcbk.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gfqvinfvy.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmkyvcnul.sHtML

[T10] Kotlin：默认参数
来源：http://blog.fanxiaobao.xyz/Article/details/ghxrlztij.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grwepwrfn.sHtML

[T11] Kotlin：协程
来源：http://baike.fanxiaobao.xyz/Article/details/ghrwgjapb.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.fanxiaobao.xyz/Article/details/gftjkxgtr.sHtML

[T12] Kotlin：解构声明
来源：http://wap.fanxiaobao.xyz/Article/details/gmodpoeap.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gbftnrjdv.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.fanxiaobao.xyz/Article/details/gbczzfcrl.sHtML

val m = mapOf("a" to 1)
来源：http://baike.fanxiaobao.xyz/Article/details/ghdeyqgkr.sHtML

[T14] Kotlin：循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gsejdolqi.sHtML

for (i in 1..10) println(i)
来源：http://read.share.fanxiaobao.xyz/Article/details/gycsexxys.sHtML

[T15] Kotlin：接口
来源：http://mobile.fanxiaobao.xyz/Article/details/gqtkwabuo.sHtML

interface Shape { fun area(): Double }
来源：http://baike.fanxiaobao.xyz/Article/details/gzwqwtxnh.sHtML

[T16] Swift：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gsznshirc.sHtML

print("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gkwelldrr.sHtML

[T17] Swift：变量与常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gockvlstp.sHtML

var a = 1;  let b = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gwaohecpo.sHtML

[T18] Swift：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/gemkryxls.sHtML

"值: \(b)"
来源：http://3g.fanxiaobao.xyz/Article/details/gtwvyxekh.sHtML

[T19] Swift：可选绑定
来源：http://m.share.fanxiaobao.xyz/Article/details/gmjtalfut.sHtML

if let n = opt { print(n) }
来源：http://baike.fanxiaobao.xyz/Article/details/gzpsrqnhj.sHtML

[T20] Swift：数组操作
来源：http://blog.fanxiaobao.xyz/Article/details/gskcaepfn.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbfeeewhe.sHtML

[T21] Swift：遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gqhjyxsol.sHtML

for x in a { print(x) }
来源：http://m.share.fanxiaobao.xyz/Article/details/grlqrnlte.sHtML

[T22] Swift：字典
来源：http://baike.fanxiaobao.xyz/Article/details/gmqcxuhmb.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfwrrwxxo.sHtML

[T23] Swift：函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdohkjlpv.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.fanxiaobao.xyz/Article/details/ghrsdqhan.sHtML

[T24] Swift：闭包
来源：http://blog.fanxiaobao.xyz/Article/details/gdsesgsqh.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.fanxiaobao.xyz/Article/details/gnipohesc.sHtML

[T25] Swift：结构体
来源：http://m.share.fanxiaobao.xyz/Article/details/gbwihmqbk.sHtML

struct P { var x: Int }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqwaxkcnz.sHtML

[T26] Swift：类与重写
来源：http://www.share.fanxiaobao.xyz/Article/details/gtrokwzfz.sHtML

class A: Base { override func f() {} }
来源：http://wap.fanxiaobao.xyz/Article/details/gqmvrtahr.sHtML


<!-- 参考信息 -->