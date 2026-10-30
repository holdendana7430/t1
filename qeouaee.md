代发 wailian999

echo "${#arr[@]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdldsvtgw.sHtML

[R20] 关联数组（字典）
来源：http://3g.fanxiaobao.xyz/Article/details/gzjcywhbw.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gjewtmnwm.sHtML

[R21] 字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gcguwrvbk.sHtML

echo "${#s}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gzbwgpanw.sHtML

[R22] 截取子串
来源：http://www.share.fanxiaobao.xyz/Article/details/gbbkwcspm.sHtML

echo "${s:0:5}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvkicnlys.sHtML

[R23] 字符串替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gvepuoyyw.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gyxpnkiap.sHtML

[R24] 大小写转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gwfyqajyh.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmserpcxh.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsggknzgn.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.fanxiaobao.xyz/Article/details/gvelrumzd.sHtML

[R26] 命令替换
来源：http://blog.fanxiaobao.xyz/Article/details/gqafevmyl.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.fanxiaobao.xyz/Article/details/gfxpmqehg.sHtML

[R27] 算术展开
来源：http://wap.fanxiaobao.xyz/Article/details/gatrghbyy.sHtML

echo $((1 + 2 * 3))
来源：http://blog.fanxiaobao.xyz/Article/details/gnxfayrjr.sHtML

[R28] 浮点运算
来源：http://wap.fanxiaobao.xyz/Article/details/gntprjfbb.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcbrbjshy.sHtML

[R29] 定义函数
来源：http://blog.fanxiaobao.xyz/Article/details/gvjpwyqfl.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.fanxiaobao.xyz/Article/details/gfqfsirej.sHtML

[R30] 函数返回状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/glrcgavpb.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfqdltyuc.sHtML

[R31] 局部变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gsvvwdwae.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gvqnxoyxe.sHtML

[R32] 参数个数校验
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnttrfyfy.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzfherkvb.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gduaxvmay.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.fanxiaobao.xyz/Article/details/getlamvpj.sHtML

[R34] 退出时清理
来源：http://read.share.fanxiaobao.xyz/Article/details/gbrzdrjem.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/gwzgdfgtd.sHtML

[R35] 后台执行并等待
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpntdgtev.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fanxiaobao.xyz/Article/details/gmiokfuzx.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdeejiotk.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.fanxiaobao.xyz/Article/details/guqfemfml.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gprbfobco.sHtML

files=$(ls -1)
来源：http://m.share.fanxiaobao.xyz/Article/details/ginbkcato.sHtML

[R38] 管道串联
来源：http://mobile.fanxiaobao.xyz/Article/details/grirbvwxz.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbagltfcd.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.fanxiaobao.xyz/Article/details/gjrbbtwbo.sHtML

cmd > out.log 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/gcbyxcdci.sHtML

[R40] 追加写日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grcfhwxls.sHtML

echo "log" >> out.log
来源：http://blog.fanxiaobao.xyz/Article/details/glxqvolql.sHtML

[R41] 丢弃输出
来源：http://blog.fanxiaobao.xyz/Article/details/goygrouxb.sHtML

cmd >/dev/null 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gwvovhtff.sHtML

[R42] 输入重定向
来源：http://www.blog.fanxiaobao.xyz/Article/details/gspukdvjs.sHtML

wc -l < a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggpgicwnh.sHtML

[R43] 按名字查找文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gbkslpxok.sHtML

find . -name "*.log" -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzcgfnxqm.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gejwosing.sHtML

find . -mtime -7 -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/gjjkcmsox.sHtML

[R45] 批量删除
来源：http://www.blog.fanxiaobao.xyz/Article/details/getfpiott.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkoalobtc.sHtML

[R46] 递归替换文件内容
来源：http://mobile.fanxiaobao.xyz/Article/details/gidviujfx.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzatmbknc.sHtML

[R47] sed 单行替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gnzysjhrx.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gbqztfcdb.sHtML

[R48] awk 取指定列
来源：http://wap.fanxiaobao.xyz/Article/details/glclstirr.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/grhfmsldp.sHtML

[R49] awk 带条件
来源：http://blog.fanxiaobao.xyz/Article/details/gnrgxqfzw.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.fanxiaobao.xyz/Article/details/gifhdnida.sHtML

[R50] awk 求和
来源：http://blog.fanxiaobao.xyz/Article/details/gyodvratw.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/giguaeucg.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gejyskgbq.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.fanxiaobao.xyz/Article/details/gazsbbwut.sHtML

[R52] 统计行数
来源：http://blog.fanxiaobao.xyz/Article/details/gydfiswxl.sHtML

wc -l a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gznerxtom.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fanxiaobao.xyz/Article/details/grzqvnupw.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.fanxiaobao.xyz/Article/details/gnsdxxnfr.sHtML

[R54] 比较两个文件
来源：http://baike.fanxiaobao.xyz/Article/details/goeoyfqzl.sHtML

diff a.txt b.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gnkbgpubu.sHtML

[R55] 压缩与解压
来源：http://m.share.fanxiaobao.xyz/Article/details/gaonbporm.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbsgsbnhr.sHtML

[R56] 远程拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/gpgumydxt.sHtML

scp file user@host:/path/
来源：http://mobile.fanxiaobao.xyz/Article/details/gblcqormk.sHtML

[R57] 远程执行命令
来源：http://blog.fanxiaobao.xyz/Article/details/goiorkjdw.sHtML

ssh user@host 'uptime'
来源：http://wap.fanxiaobao.xyz/Article/details/gzadcrpyk.sHtML

[R58] 下载文件
来源：http://m.share.fanxiaobao.xyz/Article/details/ggkherkss.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fanxiaobao.xyz/Article/details/gpjfowgdq.sHtML

[R59] 发 POST JSON
来源：http://mobile.fanxiaobao.xyz/Article/details/gafqyciyl.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fanxiaobao.xyz/Article/details/gdcorkhpl.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.fanxiaobao.xyz/Article/details/gqxkgbbft.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwlyomnlo.sHtML

[R61] 磁盘占用
来源：http://wap.fanxiaobao.xyz/Article/details/gbbtdxlau.sHtML

df -h;  du -sh *
来源：http://3g.fanxiaobao.xyz/Article/details/gusbesnic.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghmwmnhoj.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxuisdqdl.sHtML

[R63] 内存与进程
来源：http://wap.fanxiaobao.xyz/Article/details/gduvnxtph.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcnyvyrby.sHtML

[R64] 结束进程
来源：http://www.share.fanxiaobao.xyz/Article/details/giocglang.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.fanxiaobao.xyz/Article/details/gyocbhcvd.sHtML

[R65] 查看端口占用
来源：http://read.share.fanxiaobao.xyz/Article/details/gkqibifrs.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.fanxiaobao.xyz/Article/details/godoiujsu.sHtML

[R66] 定时任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/grqsfmozb.sHtML

crontab -e;  crontab -l
来源：http://read.share.fanxiaobao.xyz/Article/details/geaojtuqk.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fanxiaobao.xyz/Article/details/gwhrzrpmp.sHtML

openssl rand -hex 16
来源：http://baike.fanxiaobao.xyz/Article/details/gpbtwqums.sHtML

[R68] 计算文件校验值
来源：http://www.share.fanxiaobao.xyz/Article/details/gtdedirpy.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gxkchfmlg.sHtML

[R69] 生成随机密码
来源：http://blog.fanxiaobao.xyz/Article/details/gluoxnmsy.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fanxiaobao.xyz/Article/details/gnypwcmcd.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcsizxvim.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fanxiaobao.xyz/Article/details/gorrfobvo.sHtML

[R71] 日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gtheuskrz.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fanxiaobao.xyz/Article/details/gxzcghjep.sHtML

[R72] 等待端口就绪
来源：http://m.share.fanxiaobao.xyz/Article/details/gfhnrtzwt.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gebdlgiez.sHtML

[R73] 分割大日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghtluaubi.sHtML

split -l 1000 big.log part_
来源：http://read.share.fanxiaobao.xyz/Article/details/gldyzhavp.sHtML

[R74] 批量重命名
来源：http://wap.fanxiaobao.xyz/Article/details/gwgdrhnmy.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpuzaikyh.sHtML

[R75] 导出环境变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfxzplicf.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdgeuseqb.sHtML

[R76] 使用临时文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaijrtrse.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.fanxiaobao.xyz/Article/details/gczvsnzzs.sHtML

[R77] 读取用户输入
来源：http://baike.fanxiaobao.xyz/Article/details/grxlecoai.sHtML

read -rp "请输入: " ans
来源：http://blog.fanxiaobao.xyz/Article/details/gxxiyknbz.sHtML

[R78] 交互式菜单
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtjrfrysb.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.fanxiaobao.xyz/Article/details/geieyafeg.sHtML

[R79] 解析命令行选项
来源：http://mobile.fanxiaobao.xyz/Article/details/ggrlvsvkz.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdnidqrpr.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtcfsygwa.sHtML

time ./run.sh
来源：http://www.share.fanxiaobao.xyz/Article/details/gnkaqihya.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gukuqyixv.sHtML

S. C / C++ 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtfbccjuv.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gkejqsnxh.sHtML

[S01] C：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gxbvrsyyo.sHtML

#include <stdio.h>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcgetgxry.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gekubdpxj.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gihvdtrrg.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.fanxiaobao.xyz/Article/details/guayyjnzp.sHtML

[S03] C：读入整数
来源：http://m.share.fanxiaobao.xyz/Article/details/gjqmiltrf.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fanxiaobao.xyz/Article/details/gmlraagqk.sHtML

[S04] C：字符串复制
来源：http://3g.fanxiaobao.xyz/Article/details/gxdyszblg.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmtpqissj.sHtML

[S05] C：字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjcyxkimz.sHtML

strlen(s)
来源：http://wap.fanxiaobao.xyz/Article/details/ghuucpuxl.sHtML

[S06] C：字符串比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gbtywgscp.sHtML

strcmp(a, b) == 0
来源：http://blog.fanxiaobao.xyz/Article/details/gmnqzknuw.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpnbeqfpy.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fanxiaobao.xyz/Article/details/gveosfzte.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fanxiaobao.xyz/Article/details/gqaqbkgxf.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fanxiaobao.xyz/Article/details/gxuzzfbli.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyrcoueiw.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fanxiaobao.xyz/Article/details/gujanblqf.sHtML

[S10] C：指针与解引用
来源：http://read.share.fanxiaobao.xyz/Article/details/gcuhfayha.sHtML

int *p = &a;  *p = 5;
来源：http://blog.fanxiaobao.xyz/Article/details/gnuorjcbw.sHtML

[S11] C：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/ghokrzxoq.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fanxiaobao.xyz/Article/details/ghxtyjqra.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gfdggcgzf.sHtML

fclose(f);
来源：http://mobile.fanxiaobao.xyz/Article/details/gwejbttsq.sHtML

[S12] C：写文件
来源：http://baike.fanxiaobao.xyz/Article/details/giekbwght.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/gwwgugssv.sHtML

[S13] C：宏定义
来源：http://www.share.fanxiaobao.xyz/Article/details/gilqxmghb.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.fanxiaobao.xyz/Article/details/ghhfbabwb.sHtML

[S14] C：枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/gsmoghuhd.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fanxiaobao.xyz/Article/details/gxjzlvohw.sHtML

[S15] C：类型转换
来源：http://m.share.fanxiaobao.xyz/Article/details/ghnjyoqrz.sHtML

(double) a / b
来源：http://read.share.fanxiaobao.xyz/Article/details/gmcpmhdqm.sHtML

[S16] C：位操作置位
来源：http://m.share.fanxiaobao.xyz/Article/details/gvvngbyyx.sHtML

x |= (1 << 3);
来源：http://blog.fanxiaobao.xyz/Article/details/guxnhbwte.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyspjfndk.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.fanxiaobao.xyz/Article/details/gygawiuwc.sHtML

[S18] C：命令行参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gkiacakhh.sHtML

int main(int argc, char **argv)
来源：http://blog.fanxiaobao.xyz/Article/details/glzvjstay.sHtML

[S19] C：快速排序
来源：http://mobile.fanxiaobao.xyz/Article/details/glzuclztx.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/gjtazripx.sHtML

[S20] C：二分查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcxnlssrh.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyjrorxdb.sHtML

[S21] C：字符类别判断
来源：http://www.share.fanxiaobao.xyz/Article/details/ghaprpatb.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.fanxiaobao.xyz/Article/details/geariwpyt.sHtML

[S22] C：字符串转数字
来源：http://3g.fanxiaobao.xyz/Article/details/glvidgqtc.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fanxiaobao.xyz/Article/details/gfobcheju.sHtML

[S23] C：随机数
来源：http://wap.fanxiaobao.xyz/Article/details/gadnkhrxw.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.fanxiaobao.xyz/Article/details/glmaciscn.sHtML

[S24] C：获取本地时间
来源：http://baike.fanxiaobao.xyz/Article/details/gwpjcibtu.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fanxiaobao.xyz/Article/details/ggqxgbsrg.sHtML

[S25] C：内存拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/giliwkdzn.sHtML

memcpy(dst, src, n);
来源：http://3g.fanxiaobao.xyz/Article/details/gdbsskjci.sHtML

[S26] C：内存清零
来源：http://baike.fanxiaobao.xyz/Article/details/grkcfameq.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fanxiaobao.xyz/Article/details/gpzkuawqz.sHtML

[S27] C：定义常量
来源：http://mobile.fanxiaobao.xyz/Article/details/gzjbgwyrp.sHtML

const double PI = 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/gxylnmwlt.sHtML

[S28] C：静态变量
来源：http://blog.fanxiaobao.xyz/Article/details/gzkgeplvi.sHtML

static int counter = 0;
来源：http://3g.fanxiaobao.xyz/Article/details/gmxspteut.sHtML

[S29] C：变参函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghtgbdfrr.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fanxiaobao.xyz/Article/details/gnesmfvkj.sHtML

[S30] C：头文件保护
来源：http://3g.fanxiaobao.xyz/Article/details/ggruxyjut.sHtML

#ifndef X_H
来源：http://blog.fanxiaobao.xyz/Article/details/grmnyifvq.sHtML

#define X_H
来源：http://3g.fanxiaobao.xyz/Article/details/gkkuqirrb.sHtML

#endif
来源：http://3g.fanxiaobao.xyz/Article/details/glqavvlug.sHtML

[S31] C++：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/ggfxrlcis.sHtML

#include <iostream>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvkdpufyr.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvqrrhick.sHtML

[S32] C++：字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/grntfwnlp.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.fanxiaobao.xyz/Article/details/gjtowztns.sHtML

[S33] C++：vector 增删
来源：http://blog.fanxiaobao.xyz/Article/details/gkdkgyrgf.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gxwdiosuz.sHtML

[S34] C++：遍历 vector
来源：http://mobile.fanxiaobao.xyz/Article/details/grvxtmrpf.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.fanxiaobao.xyz/Article/details/gqfzmhqko.sHtML

[S35] C++：map
来源：http://blog.fanxiaobao.xyz/Article/details/gmuzwxlmf.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gormcguze.sHtML

[S36] C++：unordered_map
来源：http://mobile.fanxiaobao.xyz/Article/details/gmxukfppw.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/grmblnvrt.sHtML

[S37] C++：set
来源：http://3g.fanxiaobao.xyz/Article/details/gyzcliklg.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gylvwmdfg.sHtML

[S38] C++：排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gzguvosxk.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.fanxiaobao.xyz/Article/details/gufgrubrc.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.fanxiaobao.xyz/Article/details/ghyqosiqk.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glcrppavp.sHtML

[S40] C++：查找元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gkgzywfeu.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gagofdutg.sHtML

[S41] C++：类与构造函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gdwfsklcb.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gugkjdrra.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fanxiaobao.xyz/Article/details/gykecllxw.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.fanxiaobao.xyz/Article/details/goodtqsri.sHtML

[S43] C++：智能指针
来源：http://read.share.fanxiaobao.xyz/Article/details/gxqzrfouf.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.fanxiaobao.xyz/Article/details/gxzffaqly.sHtML

[S44] C++：引用传参
来源：http://m.share.fanxiaobao.xyz/Article/details/glcvpxrzv.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gotuqkqag.sHtML

[S45] C++：lambda
来源：http://baike.fanxiaobao.xyz/Article/details/gypoltnul.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/geijwjmmi.sHtML

[S46] C++：函数模板
来源：http://baike.fanxiaobao.xyz/Article/details/goymzhnmw.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtoxypukz.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gdobxdyon.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.fanxiaobao.xyz/Article/details/gylxoeiro.sHtML

[S48] C++：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gfudgkiln.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcpklsxck.sHtML

while (std::getline(in, line)) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gjdmezche.sHtML

[S49] C++：写文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gqwbfcvtv.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fanxiaobao.xyz/Article/details/gfhwutgfc.sHtML

[S50] C++：格式化数字
来源：http://read.share.fanxiaobao.xyz/Article/details/gwpgllpew.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghxmwbwba.sHtML

[S51] C++：显式类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gmqejenuf.sHtML

static_cast<double>(a) / b
来源：http://baike.fanxiaobao.xyz/Article/details/gdlrdmvms.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwgxrbpnt.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmqruslfu.sHtML

[S53] C++：移动语义
来源：http://wap.fanxiaobao.xyz/Article/details/gwpthopnw.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.fanxiaobao.xyz/Article/details/gaggfvbcr.sHtML

[S54] C++：异常处理
来源：http://3g.fanxiaobao.xyz/Article/details/gcdgluald.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gvyqalnjc.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fanxiaobao.xyz/Article/details/glisjbbva.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.fanxiaobao.xyz/Article/details/gmlvdaesl.sHtML

[S56] C++：optional
来源：http://mobile.fanxiaobao.xyz/Article/details/gvccxizpn.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.fanxiaobao.xyz/Article/details/ghippkisv.sHtML

[S57] C++：编译期常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gmfnczcuy.sHtML

constexpr int N = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjuporrjx.sHtML

[S58] C++：命名空间
来源：http://www.share.fanxiaobao.xyz/Article/details/glnqbzszo.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.fanxiaobao.xyz/Article/details/gclhnbdjc.sHtML

[S59] C++：静态断言
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmqpetune.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.fanxiaobao.xyz/Article/details/goidfvmue.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.fanxiaobao.xyz/Article/details/ggqumbowg.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.fanxiaobao.xyz/Article/details/glrphxjjf.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gitasedjd.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guvlhxpcm.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gyrczwjuy.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvevjwfkv.sHtML

println("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gpclgqhvk.sHtML

[T02] Kotlin：变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gjnetafld.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.fanxiaobao.xyz/Article/details/gvmfvjuda.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyouzzeek.sHtML

"值: $b"
来源：http://m.share.fanxiaobao.xyz/Article/details/gmucibaeg.sHtML

[T04] Kotlin：空安全
来源：http://blog.fanxiaobao.xyz/Article/details/gqpbbvvio.sHtML

val n: String? = null;  n?.length
来源：http://blog.fanxiaobao.xyz/Article/details/gtvnyytut.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.fanxiaobao.xyz/Article/details/gnhtbommc.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.fanxiaobao.xyz/Article/details/gmoakedml.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqrougkmt.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gcfyrxrpr.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/gyxlvxhjx.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gitodtngd.sHtML

[T08] Kotlin：数据类
来源：http://baike.fanxiaobao.xyz/Article/details/gvyyhuxeb.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.fanxiaobao.xyz/Article/details/geoziwkft.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gcpbdsnig.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwxpxsqrs.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.fanxiaobao.xyz/Article/details/ghxzbtjmf.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.fanxiaobao.xyz/Article/details/gapcbgvif.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzkhxwsjq.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.fanxiaobao.xyz/Article/details/gzxlugnyo.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.fanxiaobao.xyz/Article/details/glgldewuv.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gshtyzumm.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.fanxiaobao.xyz/Article/details/gvmxmicdr.sHtML

val m = mapOf("a" to 1)
来源：http://baike.fanxiaobao.xyz/Article/details/gfledysik.sHtML

[T14] Kotlin：循环
来源：http://3g.fanxiaobao.xyz/Article/details/gxlefrqun.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbbfhkrmm.sHtML

[T15] Kotlin：接口
来源：http://mobile.fanxiaobao.xyz/Article/details/gyhxqxdfz.sHtML

interface Shape { fun area(): Double }
来源：http://3g.fanxiaobao.xyz/Article/details/gwpvosjqa.sHtML

[T16] Swift：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gwbiqdnez.sHtML

print("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gblemannz.sHtML

[T17] Swift：变量与常量
来源：http://mobile.fanxiaobao.xyz/Article/details/gqoeozxmi.sHtML

var a = 1;  let b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/grblflrbf.sHtML

[T18] Swift：字符串插值
来源：http://baike.fanxiaobao.xyz/Article/details/geejmrgtl.sHtML

"值: \(b)"
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghjlptcrs.sHtML

[T19] Swift：可选绑定
来源：http://m.share.fanxiaobao.xyz/Article/details/gfuydwbnv.sHtML

if let n = opt { print(n) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gdpgadzrb.sHtML

[T20] Swift：数组操作
来源：http://blog.fanxiaobao.xyz/Article/details/glshizfoh.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.fanxiaobao.xyz/Article/details/grupiiqcy.sHtML

[T21] Swift：遍历
来源：http://blog.fanxiaobao.xyz/Article/details/giszzwkxp.sHtML

for x in a { print(x) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gxzdsytjn.sHtML

[T22] Swift：字典
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqxmhhnhq.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gfazzuwha.sHtML


<!-- 参考信息 -->