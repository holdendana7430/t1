代发 wailian999

echo "${#arr[@]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/glgqcszwl.sHtML

[R20] 关联数组（字典）
来源：http://wap.fanxiaobao.xyz/Article/details/gdwitfqfj.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/getzxbbpc.sHtML

[R21] 字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpxhdzbgo.sHtML

echo "${#s}"
来源：http://wap.fanxiaobao.xyz/Article/details/gvezmtmlg.sHtML

[R22] 截取子串
来源：http://baike.fanxiaobao.xyz/Article/details/gvuvwlisr.sHtML

echo "${s:0:5}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghykehhsf.sHtML

[R23] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/gfxmauexd.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gibwjxluj.sHtML

[R24] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/gfcruzskp.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gnyvcdofg.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.fanxiaobao.xyz/Article/details/gvouxkncg.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.fanxiaobao.xyz/Article/details/gbyvvhwki.sHtML

[R26] 命令替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gfeeyqmax.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbhjdgjwj.sHtML

[R27] 算术展开
来源：http://baike.fanxiaobao.xyz/Article/details/gvbxbravl.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fanxiaobao.xyz/Article/details/gpeyjxyze.sHtML

[R28] 浮点运算
来源：http://3g.fanxiaobao.xyz/Article/details/gcsboxtel.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fanxiaobao.xyz/Article/details/gvagriayh.sHtML

[R29] 定义函数
来源：http://www.share.fanxiaobao.xyz/Article/details/guqveofjn.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gvfamchli.sHtML

[R30] 函数返回状态码
来源：http://mobile.fanxiaobao.xyz/Article/details/gjccifaqi.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.fanxiaobao.xyz/Article/details/gnloivaob.sHtML

[R31] 局部变量
来源：http://read.share.fanxiaobao.xyz/Article/details/getsexjlt.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gfpebnjyu.sHtML

[R32] 参数个数校验
来源：http://www.share.fanxiaobao.xyz/Article/details/gfnadhulj.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbqkmalxr.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.fanxiaobao.xyz/Article/details/gteqpfovs.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.fanxiaobao.xyz/Article/details/gipxivmev.sHtML

[R34] 退出时清理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gajnjwwnx.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxafqrymi.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmgexxnxr.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fanxiaobao.xyz/Article/details/gfsolknzm.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkalnnfgg.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.fanxiaobao.xyz/Article/details/gxxcuqohi.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fanxiaobao.xyz/Article/details/glsukrmhn.sHtML

files=$(ls -1)
来源：http://baike.fanxiaobao.xyz/Article/details/gfigmwyom.sHtML

[R38] 管道串联
来源：http://mobile.fanxiaobao.xyz/Article/details/gucqzkonl.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fanxiaobao.xyz/Article/details/gtvmdblyv.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.fanxiaobao.xyz/Article/details/grrwnplxn.sHtML

cmd > out.log 2>&1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsgodszvl.sHtML

[R40] 追加写日志
来源：http://baike.fanxiaobao.xyz/Article/details/govlbgiev.sHtML

echo "log" >> out.log
来源：http://read.share.fanxiaobao.xyz/Article/details/gubffkadt.sHtML

[R41] 丢弃输出
来源：http://3g.fanxiaobao.xyz/Article/details/gfqkpnpts.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/gsatiwvvn.sHtML

[R42] 输入重定向
来源：http://wap.fanxiaobao.xyz/Article/details/gxyduwbqd.sHtML

wc -l < a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glmyfgdkl.sHtML

[R43] 按名字查找文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gzrjhttph.sHtML

find . -name "*.log" -type f
来源：http://baike.fanxiaobao.xyz/Article/details/gtrojyuym.sHtML

[R44] 按修改时间查找
来源：http://read.share.fanxiaobao.xyz/Article/details/gogvgrpiy.sHtML

find . -mtime -7 -type f
来源：http://baike.fanxiaobao.xyz/Article/details/gujmiobxs.sHtML

[R45] 批量删除
来源：http://mobile.fanxiaobao.xyz/Article/details/gmsoluaak.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fanxiaobao.xyz/Article/details/gnkiehtkq.sHtML

[R46] 递归替换文件内容
来源：http://wap.fanxiaobao.xyz/Article/details/gxwqmcwlh.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fanxiaobao.xyz/Article/details/graxfwhtp.sHtML

[R47] sed 单行替换
来源：http://wap.fanxiaobao.xyz/Article/details/gilfbqmin.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gykwzqnad.sHtML

[R48] awk 取指定列
来源：http://baike.fanxiaobao.xyz/Article/details/gzyouywde.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gpigvjuvd.sHtML

[R49] awk 带条件
来源：http://m.share.fanxiaobao.xyz/Article/details/ghvgdlaiw.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fanxiaobao.xyz/Article/details/gsihliydw.sHtML

[R50] awk 求和
来源：http://blog.fanxiaobao.xyz/Article/details/gjfvyfszx.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gkqqvpqad.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gshkarexj.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.fanxiaobao.xyz/Article/details/gwnnfoqdo.sHtML

[R52] 统计行数
来源：http://mobile.fanxiaobao.xyz/Article/details/gfdgzsvgq.sHtML

wc -l a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gcfuqzclw.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fanxiaobao.xyz/Article/details/gatubwycz.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fanxiaobao.xyz/Article/details/gctbwraqm.sHtML

[R54] 比较两个文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gtvxuhvpg.sHtML

diff a.txt b.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/giibwistc.sHtML

[R55] 压缩与解压
来源：http://wap.fanxiaobao.xyz/Article/details/gleokrxvl.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.fanxiaobao.xyz/Article/details/gpvntmkur.sHtML

[R56] 远程拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gmktfvbqi.sHtML

scp file user@host:/path/
来源：http://m.share.fanxiaobao.xyz/Article/details/glyeqfgmr.sHtML

[R57] 远程执行命令
来源：http://read.share.fanxiaobao.xyz/Article/details/grwiuqmap.sHtML

ssh user@host 'uptime'
来源：http://3g.fanxiaobao.xyz/Article/details/gsygiaump.sHtML

[R58] 下载文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gaxgewpfu.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fanxiaobao.xyz/Article/details/gtclqzvxs.sHtML

[R59] 发 POST JSON
来源：http://wap.fanxiaobao.xyz/Article/details/goobzcguq.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fanxiaobao.xyz/Article/details/gqcufibuq.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.fanxiaobao.xyz/Article/details/gidraqaef.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fanxiaobao.xyz/Article/details/gucogzniu.sHtML

[R61] 磁盘占用
来源：http://3g.fanxiaobao.xyz/Article/details/gjfydrqlb.sHtML

df -h;  du -sh *
来源：http://wap.fanxiaobao.xyz/Article/details/gdmslndcf.sHtML

[R62] 找最占空间的文件
来源：http://baike.fanxiaobao.xyz/Article/details/gfqsmwkyu.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fanxiaobao.xyz/Article/details/gholnytdg.sHtML

[R63] 内存与进程
来源：http://www.share.fanxiaobao.xyz/Article/details/gtuvbltoa.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.fanxiaobao.xyz/Article/details/grxusabgr.sHtML

[R64] 结束进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvnykdmyf.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.fanxiaobao.xyz/Article/details/ggzzxuhgc.sHtML

[R65] 查看端口占用
来源：http://mobile.fanxiaobao.xyz/Article/details/gsciekpky.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghuhbxaqd.sHtML

[R66] 定时任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtyialpgj.sHtML

crontab -e;  crontab -l
来源：http://blog.fanxiaobao.xyz/Article/details/gsxgvopkw.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fanxiaobao.xyz/Article/details/glfjiltkh.sHtML

openssl rand -hex 16
来源：http://read.share.fanxiaobao.xyz/Article/details/gkthygicx.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggrybimhc.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gdxbaiije.sHtML

[R69] 生成随机密码
来源：http://www.share.fanxiaobao.xyz/Article/details/gqceivmdm.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fanxiaobao.xyz/Article/details/gxoslsnrr.sHtML

[R70] 时间戳与互转
来源：http://mobile.fanxiaobao.xyz/Article/details/gfknbioeo.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggplfuyiw.sHtML

[R71] 日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdlzgpfsg.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnpmmxfvn.sHtML

[R72] 等待端口就绪
来源：http://wap.fanxiaobao.xyz/Article/details/gxrcrranm.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/gkksknzrj.sHtML

[R73] 分割大日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gfiljdhxx.sHtML

split -l 1000 big.log part_
来源：http://wap.fanxiaobao.xyz/Article/details/gwfnzortp.sHtML

[R74] 批量重命名
来源：http://wap.fanxiaobao.xyz/Article/details/gifkrusgj.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/ggrkmuskm.sHtML

[R75] 导出环境变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcbxfcivl.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.fanxiaobao.xyz/Article/details/ghrkirfvy.sHtML

[R76] 使用临时文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfaknzgkg.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/gwnwyfjnu.sHtML

[R77] 读取用户输入
来源：http://wap.fanxiaobao.xyz/Article/details/gfyjsglvi.sHtML

read -rp "请输入: " ans
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghmdozhun.sHtML

[R78] 交互式菜单
来源：http://baike.fanxiaobao.xyz/Article/details/gvlrvwjxm.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.fanxiaobao.xyz/Article/details/gtvaxfyxn.sHtML

[R79] 解析命令行选项
来源：http://read.share.fanxiaobao.xyz/Article/details/gylgwljix.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fanxiaobao.xyz/Article/details/gxjvsmovp.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fanxiaobao.xyz/Article/details/gurjolfkk.sHtML

time ./run.sh
来源：http://3g.fanxiaobao.xyz/Article/details/gvivamonz.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/glzkfwbit.sHtML

S. C / C++ 专题
来源：http://baike.fanxiaobao.xyz/Article/details/ghffglldz.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gnrgnwqlj.sHtML

[S01] C：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gqyuttpgh.sHtML

#include <stdio.h>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqoybdaxe.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghcbintng.sHtML

[S02] C：变量与格式化输出
来源：http://baike.fanxiaobao.xyz/Article/details/gcocbtdsi.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.fanxiaobao.xyz/Article/details/glerieonw.sHtML

[S03] C：读入整数
来源：http://baike.fanxiaobao.xyz/Article/details/gemyubnow.sHtML

int x; scanf("%d", &x);
来源：http://wap.fanxiaobao.xyz/Article/details/gurqwbnny.sHtML

[S04] C：字符串复制
来源：http://mobile.fanxiaobao.xyz/Article/details/gmrzkxshx.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fanxiaobao.xyz/Article/details/ggspncgah.sHtML

[S05] C：字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gxfeqambu.sHtML

strlen(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gitrxglci.sHtML

[S06] C：字符串比较
来源：http://blog.fanxiaobao.xyz/Article/details/gltnsfzof.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyvkplywu.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/guwvccygs.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqfgjataa.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfosqtmov.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gesnuwrbp.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fanxiaobao.xyz/Article/details/gvadofgyk.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fanxiaobao.xyz/Article/details/gvdcjnpfb.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnibjhprx.sHtML

int *p = &a;  *p = 5;
来源：http://blog.fanxiaobao.xyz/Article/details/gutdeaumx.sHtML

[S11] C：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/ghdgdwknl.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fanxiaobao.xyz/Article/details/gxcugxzgg.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggyarajex.sHtML

fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/gfxobhusv.sHtML

[S12] C：写文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gvhoaiwmi.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghgbhonmm.sHtML

[S13] C：宏定义
来源：http://blog.fanxiaobao.xyz/Article/details/guqwahpdg.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.fanxiaobao.xyz/Article/details/gylezjdcg.sHtML

[S14] C：枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/gboytldnb.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.fanxiaobao.xyz/Article/details/gncwgmkap.sHtML

[S15] C：类型转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gpdwmmnji.sHtML

(double) a / b
来源：http://wap.fanxiaobao.xyz/Article/details/gmsuiijqc.sHtML

[S16] C：位操作置位
来源：http://www.share.fanxiaobao.xyz/Article/details/getbfjzab.sHtML

x |= (1 << 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/ghhumjmoy.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gkcbltgnc.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.fanxiaobao.xyz/Article/details/gfuxprqhk.sHtML

[S18] C：命令行参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gxficzeac.sHtML

int main(int argc, char **argv)
来源：http://blog.fanxiaobao.xyz/Article/details/gaxufswrz.sHtML

[S19] C：快速排序
来源：http://read.share.fanxiaobao.xyz/Article/details/ghnvjcuhc.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/gqwqdgggx.sHtML

[S20] C：二分查找
来源：http://blog.fanxiaobao.xyz/Article/details/gsllzcyqw.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/gqcayhdwd.sHtML

[S21] C：字符类别判断
来源：http://www.share.fanxiaobao.xyz/Article/details/gjmuzosiw.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fanxiaobao.xyz/Article/details/ghnzjagdv.sHtML

[S22] C：字符串转数字
来源：http://mobile.fanxiaobao.xyz/Article/details/gcggglena.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fanxiaobao.xyz/Article/details/gysjdfbdz.sHtML

[S23] C：随机数
来源：http://baike.fanxiaobao.xyz/Article/details/grlbbrulm.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggtrqqjte.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxuxyxdbl.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.fanxiaobao.xyz/Article/details/geswdiklf.sHtML

[S25] C：内存拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gnnaxoeln.sHtML

memcpy(dst, src, n);
来源：http://3g.fanxiaobao.xyz/Article/details/gvmftefxz.sHtML

[S26] C：内存清零
来源：http://www.share.fanxiaobao.xyz/Article/details/gbawysghe.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/girxrhqnl.sHtML

[S27] C：定义常量
来源：http://baike.fanxiaobao.xyz/Article/details/gwtqesmbq.sHtML

const double PI = 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gsmxykpmy.sHtML

[S28] C：静态变量
来源：http://blog.fanxiaobao.xyz/Article/details/glcqvcaqd.sHtML

static int counter = 0;
来源：http://read.share.fanxiaobao.xyz/Article/details/gpjlffxfa.sHtML

[S29] C：变参函数
来源：http://blog.fanxiaobao.xyz/Article/details/gemwdlrpd.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.fanxiaobao.xyz/Article/details/goiyqfawz.sHtML

[S30] C：头文件保护
来源：http://read.share.fanxiaobao.xyz/Article/details/gatrtbbyp.sHtML

#ifndef X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gcnhgtmbg.sHtML

#define X_H
来源：http://blog.fanxiaobao.xyz/Article/details/gmfcwasxo.sHtML

#endif
来源：http://read.share.fanxiaobao.xyz/Article/details/glimnnxrt.sHtML

[S31] C++：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gndxmybft.sHtML

#include <iostream>
来源：http://www.share.fanxiaobao.xyz/Article/details/gxkykmbgz.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gdoutsqpq.sHtML

[S32] C++：字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gejbrnrhg.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fanxiaobao.xyz/Article/details/gceupujcd.sHtML

[S33] C++：vector 增删
来源：http://mobile.fanxiaobao.xyz/Article/details/gvpykwsmc.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gztwzovwr.sHtML

[S34] C++：遍历 vector
来源：http://3g.fanxiaobao.xyz/Article/details/gwndengxd.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/ghiobroqr.sHtML

[S35] C++：map
来源：http://3g.fanxiaobao.xyz/Article/details/ggsdujqfz.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gutwnovny.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gapzjacgm.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxolnadbn.sHtML

[S37] C++：set
来源：http://mobile.fanxiaobao.xyz/Article/details/gdmrdeobj.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmfmrkhkt.sHtML

[S38] C++：排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmxtxcycr.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.fanxiaobao.xyz/Article/details/ggdhjfhna.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gzslvnqui.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.fanxiaobao.xyz/Article/details/grlmufvot.sHtML

[S40] C++：查找元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gssralmii.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gkcpeafut.sHtML

[S41] C++：类与构造函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gsgwwtqoc.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fanxiaobao.xyz/Article/details/gzddjwhfu.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fanxiaobao.xyz/Article/details/gxqxquulq.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fanxiaobao.xyz/Article/details/gpysujbit.sHtML

[S43] C++：智能指针
来源：http://www.share.fanxiaobao.xyz/Article/details/grsxxodse.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fanxiaobao.xyz/Article/details/ghzaaasev.sHtML

[S44] C++：引用传参
来源：http://wap.fanxiaobao.xyz/Article/details/ghqczhuvn.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghswedqpo.sHtML

[S45] C++：lambda
来源：http://www.share.fanxiaobao.xyz/Article/details/gdbzvbudi.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.fanxiaobao.xyz/Article/details/grevfjezk.sHtML

[S46] C++：函数模板
来源：http://read.share.fanxiaobao.xyz/Article/details/guyfcjxeo.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.fanxiaobao.xyz/Article/details/ghhlsucyo.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gxfhhakrm.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjqbrtuwn.sHtML

[S48] C++：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/ghpgyjpid.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwajbdary.sHtML

while (std::getline(in, line)) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gurdwiyub.sHtML

[S49] C++：写文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gczcouovv.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.fanxiaobao.xyz/Article/details/gvxjuvefu.sHtML

[S50] C++：格式化数字
来源：http://blog.fanxiaobao.xyz/Article/details/gswmzelqu.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gwwbaszlc.sHtML

[S51] C++：显式类型转换
来源：http://baike.fanxiaobao.xyz/Article/details/golqklqjj.sHtML

static_cast<double>(a) / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdkjyqldx.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gihyefpuk.sHtML

int size() const noexcept { return n_; }
来源：http://baike.fanxiaobao.xyz/Article/details/gxqrctibi.sHtML

[S53] C++：移动语义
来源：http://baike.fanxiaobao.xyz/Article/details/gdrhzvuwx.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.fanxiaobao.xyz/Article/details/gcncissna.sHtML

[S54] C++：异常处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqnurpjbc.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/goknhzfov.sHtML

[S55] C++：结构化绑定
来源：http://m.share.fanxiaobao.xyz/Article/details/gzcgjplpt.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.fanxiaobao.xyz/Article/details/glinodzsj.sHtML

[S56] C++：optional
来源：http://blog.fanxiaobao.xyz/Article/details/gtbqyurtg.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gmbdcmnkn.sHtML

[S57] C++：编译期常量
来源：http://baike.fanxiaobao.xyz/Article/details/gpmieyitl.sHtML

constexpr int N = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcmzulqwc.sHtML

[S58] C++：命名空间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjteqhpxy.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.fanxiaobao.xyz/Article/details/gmhqbnezm.sHtML

[S59] C++：静态断言
来源：http://m.share.fanxiaobao.xyz/Article/details/gtgwwaizp.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.fanxiaobao.xyz/Article/details/gmigjefme.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbvbhekos.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkrfzcech.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gwkryjnit.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fanxiaobao.xyz/Article/details/giczfkejm.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gkrvitqky.sHtML

[T01] Kotlin：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gkuohgyrh.sHtML

println("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gwbrtojrl.sHtML

[T02] Kotlin：变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gkhminpiy.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.fanxiaobao.xyz/Article/details/ggjbzhnvj.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.fanxiaobao.xyz/Article/details/ggfmboddd.sHtML

"值: $b"
来源：http://read.share.fanxiaobao.xyz/Article/details/ghqskzvrc.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmboeflpb.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzaybsfzx.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfrrqiynv.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.fanxiaobao.xyz/Article/details/gagsxsnji.sHtML

[T06] Kotlin：集合映射
来源：http://blog.fanxiaobao.xyz/Article/details/gnljoldht.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gvnjmoibc.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/giwukusip.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfluzzpvj.sHtML

[T08] Kotlin：数据类
来源：http://wap.fanxiaobao.xyz/Article/details/grjggqcim.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqsuceerh.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.fanxiaobao.xyz/Article/details/gpsmcgkvb.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.fanxiaobao.xyz/Article/details/gcdxhjkqp.sHtML

[T10] Kotlin：默认参数
来源：http://wap.fanxiaobao.xyz/Article/details/gzzxskjwu.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggnkovnsw.sHtML

[T11] Kotlin：协程
来源：http://m.share.fanxiaobao.xyz/Article/details/gdpuggxdb.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.fanxiaobao.xyz/Article/details/gcyvazjpe.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.fanxiaobao.xyz/Article/details/gfizelmuf.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gutudhgfh.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.fanxiaobao.xyz/Article/details/gcorgbmgo.sHtML

val m = mapOf("a" to 1)
来源：http://blog.fanxiaobao.xyz/Article/details/gxhjvnplo.sHtML

[T14] Kotlin：循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gdvrmsocf.sHtML

for (i in 1..10) println(i)
来源：http://baike.fanxiaobao.xyz/Article/details/gcoufawpt.sHtML

[T15] Kotlin：接口
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzpjyrxyj.sHtML

interface Shape { fun area(): Double }
来源：http://3g.fanxiaobao.xyz/Article/details/gxfplikjr.sHtML

[T16] Swift：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gkmoxzhkd.sHtML

print("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gegamjtlq.sHtML

[T17] Swift：变量与常量
来源：http://blog.fanxiaobao.xyz/Article/details/gexhhqhbu.sHtML

var a = 1;  let b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gpmwznvme.sHtML

[T18] Swift：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/guxnztvsp.sHtML

"值: \(b)"
来源：http://m.share.fanxiaobao.xyz/Article/details/gfapudybl.sHtML

[T19] Swift：可选绑定
来源：http://read.share.fanxiaobao.xyz/Article/details/gisdsexwu.sHtML

if let n = opt { print(n) }
来源：http://3g.fanxiaobao.xyz/Article/details/ggwsqofgd.sHtML

[T20] Swift：数组操作
来源：http://baike.fanxiaobao.xyz/Article/details/gzpacmdkc.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grtusyqiw.sHtML

[T21] Swift：遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gxmbajton.sHtML

for x in a { print(x) }
来源：http://baike.fanxiaobao.xyz/Article/details/guhxpezcj.sHtML

[T22] Swift：字典
来源：http://blog.fanxiaobao.xyz/Article/details/gcrfujcez.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gwggtctdc.sHtML


<!-- 参考信息 -->