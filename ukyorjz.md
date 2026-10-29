代发 wailian999

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.zdbjq.cn/Article/details/gicgkvdjr.sHtML

[R16] until 等待条件
来源：http://www.blog.zdbjq.cn/Article/details/gnibpehoi.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.zdbjq.cn/Article/details/gdsnrkeyv.sHtML

[R17] 数组定义与取值
来源：http://m.share.fehbvm.com/Article/details/gytfgvtwa.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.hesvh.cn/Article/details/gbpskvklc.sHtML

[R18] 遍历数组
来源：http://baike.zdbjq.cn/Article/details/gxqjqxfbp.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.hesvh.cn/Article/details/gdatusdwu.sHtML

[R19] 数组长度
来源：http://www.m.share.zdbjq.cn/Article/details/ghczqzayj.sHtML

echo "${#arr[@]}"
来源：http://www.share.hesvh.cn/Article/details/gxpixszvr.sHtML

[R20] 关联数组（字典）
来源：http://blog.zdbjq.cn/Article/details/gclbgrtfg.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.hesvh.cn/Article/details/gauptzmsw.sHtML

[R21] 字符串长度
来源：http://baike.fehbvm.com/Article/details/gldrptqfo.sHtML

echo "${#s}"
来源：http://baike.zdbjq.cn/Article/details/gtoncrxqx.sHtML

[R22] 截取子串
来源：http://read.share.zdbjq.cn/Article/details/gegftpvyr.sHtML

echo "${s:0:5}"
来源：http://blog.fehbvm.com/Article/details/grbqubuoy.sHtML

[R23] 字符串替换
来源：http://wap.fehbvm.com/Article/details/gmeqxkkwj.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.zdbjq.cn/Article/details/giaypeuhl.sHtML

[R24] 大小写转换
来源：http://baike.zdbjq.cn/Article/details/gcmbcuclb.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.hesvh.cn/Article/details/gtzedfdhu.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.zdbjq.cn/Article/details/gqrrhjzki.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.zdbjq.cn/Article/details/gmojtkuon.sHtML

[R26] 命令替换
来源：http://wap.zdbjq.cn/Article/details/gojpgrvzz.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.hesvh.cn/Article/details/gllxurknk.sHtML

[R27] 算术展开
来源：http://blog.hesvh.cn/Article/details/glogupmdd.sHtML

echo $((1 + 2 * 3))
来源：http://wap.zdbjq.cn/Article/details/ghdxgjjlf.sHtML

[R28] 浮点运算
来源：http://baike.hesvh.cn/Article/details/ggxhjucgt.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.zdbjq.cn/Article/details/gszjfxnfd.sHtML

[R29] 定义函数
来源：http://read.share.hesvh.cn/Article/details/gsrihbvah.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.hesvh.cn/Article/details/gjfsaqbgm.sHtML

[R30] 函数返回状态码
来源：http://read.share.zdbjq.cn/Article/details/ggcvchbor.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.zdbjq.cn/Article/details/gzfeyopti.sHtML

[R31] 局部变量
来源：http://m.share.hesvh.cn/Article/details/gtrrffrsi.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.zdbjq.cn/Article/details/gxaqgonib.sHtML

[R32] 参数个数校验
来源：http://wap.zdbjq.cn/Article/details/gchpajxgz.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.hesvh.cn/Article/details/gthwmurfo.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.hesvh.cn/Article/details/gxpuqnszd.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.zdbjq.cn/Article/details/gdtecwxmg.sHtML

[R34] 退出时清理
来源：http://read.share.zdbjq.cn/Article/details/gkqmrtkwh.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fehbvm.com/Article/details/gletwtbks.sHtML

[R35] 后台执行并等待
来源：http://read.share.fehbvm.com/Article/details/guelocnbp.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.fehbvm.com/Article/details/gvrytaror.sHtML

[R36] 并发执行多个任务
来源：http://blog.zdbjq.cn/Article/details/gtqdnpppz.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.hesvh.cn/Article/details/gobukklkv.sHtML

[R37] 把输出赋给变量
来源：http://3g.hesvh.cn/Article/details/gigbicgdy.sHtML

files=$(ls -1)
来源：http://read.share.fehbvm.com/Article/details/gbkpdezkk.sHtML

[R38] 管道串联
来源：http://blog.fehbvm.com/Article/details/gbzojcysf.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.hesvh.cn/Article/details/gzywwkpqj.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.hesvh.cn/Article/details/gozshzdks.sHtML

cmd > out.log 2>&1
来源：http://read.share.zdbjq.cn/Article/details/gmyawxyjp.sHtML

[R40] 追加写日志
来源：http://baike.zdbjq.cn/Article/details/ghpqdvtts.sHtML

echo "log" >> out.log
来源：http://www.blog.fehbvm.com/Article/details/gjmrzeuqo.sHtML

[R41] 丢弃输出
来源：http://blog.hesvh.cn/Article/details/gluiujacx.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.fehbvm.com/Article/details/gebyhywkp.sHtML

[R42] 输入重定向
来源：http://baike.hesvh.cn/Article/details/gzssnuodd.sHtML

wc -l < a.txt
来源：http://wap.hesvh.cn/Article/details/gycwxnxgn.sHtML

[R43] 按名字查找文件
来源：http://m.share.zdbjq.cn/Article/details/glgrbklcj.sHtML

find . -name "*.log" -type f
来源：http://baike.hesvh.cn/Article/details/gxaeypfxl.sHtML

[R44] 按修改时间查找
来源：http://wap.zdbjq.cn/Article/details/gjdhhzzst.sHtML

find . -mtime -7 -type f
来源：http://www.share.zdbjq.cn/Article/details/gahjiejjv.sHtML

[R45] 批量删除
来源：http://mobile.fehbvm.com/Article/details/gvcjuakoy.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.hesvh.cn/Article/details/gbglgjcct.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.hesvh.cn/Article/details/gruvrkoyq.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.hesvh.cn/Article/details/gqkqgqhnc.sHtML

[R47] sed 单行替换
来源：http://wap.hesvh.cn/Article/details/gmydiepda.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fehbvm.com/Article/details/gikrczmcv.sHtML

[R48] awk 取指定列
来源：http://baike.fehbvm.com/Article/details/gzrpohfoc.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.zdbjq.cn/Article/details/gfbeqyquz.sHtML

[R49] awk 带条件
来源：http://www.m.share.zdbjq.cn/Article/details/gjdfzjmhj.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.hesvh.cn/Article/details/gewvtmkbn.sHtML

[R50] awk 求和
来源：http://www.share.hesvh.cn/Article/details/garnhbixz.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.zdbjq.cn/Article/details/gbiynveiq.sHtML

[R51] 排序去重取前几
来源：http://m.share.zdbjq.cn/Article/details/gtfyozgtk.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.hesvh.cn/Article/details/gelbdarbj.sHtML

[R52] 统计行数
来源：http://www.blog.zdbjq.cn/Article/details/gscpvwssj.sHtML

wc -l a.txt
来源：http://blog.hesvh.cn/Article/details/gscjkfkvm.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.fehbvm.com/Article/details/ggwlheuxj.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.fehbvm.com/Article/details/gqlnvpvsr.sHtML

[R54] 比较两个文件
来源：http://www.blog.hesvh.cn/Article/details/gpwggzvpr.sHtML

diff a.txt b.txt
来源：http://wap.fehbvm.com/Article/details/gyemmxxbw.sHtML

[R55] 压缩与解压
来源：http://blog.hesvh.cn/Article/details/gzestoljq.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fehbvm.com/Article/details/gexiyexfp.sHtML

[R56] 远程拷贝
来源：http://m.share.fehbvm.com/Article/details/gskluiyrd.sHtML

scp file user@host:/path/
来源：http://baike.fehbvm.com/Article/details/gvlppwxyv.sHtML

[R57] 远程执行命令
来源：http://baike.hesvh.cn/Article/details/gxaejinrj.sHtML

ssh user@host 'uptime'
来源：http://blog.zdbjq.cn/Article/details/gsqdzlzos.sHtML

[R58] 下载文件
来源：http://3g.hesvh.cn/Article/details/gfrgitjha.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.zdbjq.cn/Article/details/gxutafeat.sHtML

[R59] 发 POST JSON
来源：http://wap.fehbvm.com/Article/details/gravjnutp.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.zdbjq.cn/Article/details/gavbarfol.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.zdbjq.cn/Article/details/gyhpbokfy.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.zdbjq.cn/Article/details/gnpldmmvn.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fehbvm.com/Article/details/gqkhsvvyw.sHtML

df -h;  du -sh *
来源：http://www.share.zdbjq.cn/Article/details/goxyzybqz.sHtML

[R62] 找最占空间的文件
来源：http://m.share.fehbvm.com/Article/details/gwepweqaf.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.zdbjq.cn/Article/details/gspqmqcyj.sHtML

[R63] 内存与进程
来源：http://www.m.share.hesvh.cn/Article/details/gplkmskwp.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.fehbvm.com/Article/details/gtguplkba.sHtML

[R64] 结束进程
来源：http://www.blog.fehbvm.com/Article/details/ghfkjvlth.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.fehbvm.com/Article/details/gjljqoeuo.sHtML

[R65] 查看端口占用
来源：http://blog.zdbjq.cn/Article/details/gbnazvzhp.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fehbvm.com/Article/details/gcjfajpwv.sHtML

[R66] 定时任务
来源：http://www.m.share.hesvh.cn/Article/details/glhhudfpq.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fehbvm.com/Article/details/gfqatimfq.sHtML

[R67] 生成随机十六进制串
来源：http://wap.zdbjq.cn/Article/details/gllukhgjq.sHtML

openssl rand -hex 16
来源：http://baike.fehbvm.com/Article/details/gengpbton.sHtML

[R68] 计算文件校验值
来源：http://www.blog.hesvh.cn/Article/details/gcffabmir.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.zdbjq.cn/Article/details/gxjgdmvis.sHtML

[R69] 生成随机密码
来源：http://mobile.zdbjq.cn/Article/details/gdlsrlhvv.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fehbvm.com/Article/details/gqnrdpbol.sHtML

[R70] 时间戳与互转
来源：http://baike.zdbjq.cn/Article/details/gtspisvpe.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.hesvh.cn/Article/details/gdrqlqdaq.sHtML

[R71] 日期格式化
来源：http://www.blog.zdbjq.cn/Article/details/gagrkljex.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.hesvh.cn/Article/details/gzeesvzri.sHtML

[R72] 等待端口就绪
来源：http://read.share.zdbjq.cn/Article/details/gbnszglpf.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.zdbjq.cn/Article/details/gyftvelzh.sHtML

[R73] 分割大日志
来源：http://blog.zdbjq.cn/Article/details/gvxncupxv.sHtML

split -l 1000 big.log part_
来源：http://read.share.hesvh.cn/Article/details/ggoovhwjq.sHtML

[R74] 批量重命名
来源：http://wap.fehbvm.com/Article/details/guqfpnyjh.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.fehbvm.com/Article/details/gpkgcyosx.sHtML

[R75] 导出环境变量
来源：http://baike.zdbjq.cn/Article/details/gkukifkip.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.fehbvm.com/Article/details/ghwnbbqln.sHtML

[R76] 使用临时文件
来源：http://baike.fehbvm.com/Article/details/gcdpwxknw.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.zdbjq.cn/Article/details/gqxmazude.sHtML

[R77] 读取用户输入
来源：http://read.share.hesvh.cn/Article/details/gubjiqfjo.sHtML

read -rp "请输入: " ans
来源：http://read.share.zdbjq.cn/Article/details/gysaeewau.sHtML

[R78] 交互式菜单
来源：http://read.share.fehbvm.com/Article/details/gmkzzzkgt.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.hesvh.cn/Article/details/gqiemhodb.sHtML

[R79] 解析命令行选项
来源：http://www.blog.zdbjq.cn/Article/details/gptclfoxt.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.zdbjq.cn/Article/details/gbpglbjks.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.fehbvm.com/Article/details/ggrzdyuuv.sHtML

time ./run.sh
来源：http://m.share.zdbjq.cn/Article/details/gnxqhhboq.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/grwqvopow.sHtML

S. C / C++ 专题
来源：http://baike.zdbjq.cn/Article/details/gwwpxpnjl.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gjqipffuc.sHtML

[S01] C：Hello World
来源：http://m.share.hesvh.cn/Article/details/ggijcqtwd.sHtML

#include <stdio.h>
来源：http://blog.zdbjq.cn/Article/details/gvbcsqjsu.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.hesvh.cn/Article/details/gfbigifer.sHtML

[S02] C：变量与格式化输出
来源：http://blog.fehbvm.com/Article/details/gdnotteno.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fehbvm.com/Article/details/ggzjvfkme.sHtML

[S03] C：读入整数
来源：http://baike.fehbvm.com/Article/details/gpyotcirc.sHtML

int x; scanf("%d", &x);
来源：http://read.share.zdbjq.cn/Article/details/gbsdqyqyu.sHtML

[S04] C：字符串复制
来源：http://3g.fehbvm.com/Article/details/gvfmqvlep.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.zdbjq.cn/Article/details/gbiqojqva.sHtML

[S05] C：字符串长度
来源：http://wap.hesvh.cn/Article/details/gwlgkjfrs.sHtML

strlen(s)
来源：http://mobile.zdbjq.cn/Article/details/gjmkqnfcm.sHtML

[S06] C：字符串比较
来源：http://wap.zdbjq.cn/Article/details/gpqsvsgcj.sHtML

strcmp(a, b) == 0
来源：http://mobile.fehbvm.com/Article/details/goxugvbpg.sHtML

[S07] C：数组遍历求和
来源：http://www.share.zdbjq.cn/Article/details/gzencvlac.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.fehbvm.com/Article/details/gvlhedico.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fehbvm.com/Article/details/gplioobxs.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fehbvm.com/Article/details/gsqkehshf.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.hesvh.cn/Article/details/garfhfyfv.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fehbvm.com/Article/details/gezrmwjsa.sHtML

[S10] C：指针与解引用
来源：http://baike.hesvh.cn/Article/details/gfotetvvc.sHtML

int *p = &a;  *p = 5;
来源：http://blog.zdbjq.cn/Article/details/gpmqoelya.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gzgdckzdn.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.hesvh.cn/Article/details/gerwvxnth.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.fehbvm.com/Article/details/gnoctsppt.sHtML

fclose(f);
来源：http://wap.fehbvm.com/Article/details/gvisdgarp.sHtML

[S12] C：写文件
来源：http://baike.fehbvm.com/Article/details/gexzulgvk.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.fehbvm.com/Article/details/gfvdawgzc.sHtML

[S13] C：宏定义
来源：http://www.m.share.fehbvm.com/Article/details/gpltmctkh.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fehbvm.com/Article/details/gszsobdex.sHtML

[S14] C：枚举
来源：http://blog.fehbvm.com/Article/details/gfishmnhf.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.hesvh.cn/Article/details/gzwxfcndu.sHtML

[S15] C：类型转换
来源：http://baike.fehbvm.com/Article/details/gmemevntr.sHtML

(double) a / b
来源：http://www.share.fehbvm.com/Article/details/gzbzhuhpu.sHtML

[S16] C：位操作置位
来源：http://www.m.share.zdbjq.cn/Article/details/gwdwucxpb.sHtML

x |= (1 << 3);
来源：http://wap.zdbjq.cn/Article/details/guxznpntc.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fehbvm.com/Article/details/gdltwylpd.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.hesvh.cn/Article/details/gebtxvxww.sHtML

[S18] C：命令行参数
来源：http://www.blog.hesvh.cn/Article/details/gibymuggo.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.zdbjq.cn/Article/details/ghkbxxgyh.sHtML

[S19] C：快速排序
来源：http://baike.zdbjq.cn/Article/details/gkrchhfkz.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.zdbjq.cn/Article/details/giowbdvge.sHtML

[S20] C：二分查找
来源：http://www.share.fehbvm.com/Article/details/geynaljqy.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.zdbjq.cn/Article/details/gcqirqmgp.sHtML

[S21] C：字符类别判断
来源：http://blog.fehbvm.com/Article/details/gmhyhidlt.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.hesvh.cn/Article/details/geagiryov.sHtML

[S22] C：字符串转数字
来源：http://blog.hesvh.cn/Article/details/gbojxqfai.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.zdbjq.cn/Article/details/glbxojrne.sHtML

[S23] C：随机数
来源：http://www.m.share.zdbjq.cn/Article/details/gkvwyzcng.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.fehbvm.com/Article/details/gqkdaqrwf.sHtML

[S24] C：获取本地时间
来源：http://www.share.fehbvm.com/Article/details/gavcfgjoh.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.zdbjq.cn/Article/details/gyqnwahdr.sHtML

[S25] C：内存拷贝
来源：http://wap.hesvh.cn/Article/details/gcsogeitk.sHtML

memcpy(dst, src, n);
来源：http://wap.hesvh.cn/Article/details/geixobxzl.sHtML

[S26] C：内存清零
来源：http://m.share.fehbvm.com/Article/details/gxaimwrjr.sHtML

memset(a, 0, sizeof a);
来源：http://wap.hesvh.cn/Article/details/gsiggtdqp.sHtML

[S27] C：定义常量
来源：http://wap.zdbjq.cn/Article/details/grdnluawe.sHtML

const double PI = 3.14159;
来源：http://3g.fehbvm.com/Article/details/gvrdvanje.sHtML

[S28] C：静态变量
来源：http://www.blog.zdbjq.cn/Article/details/gcbnadzht.sHtML

static int counter = 0;
来源：http://3g.hesvh.cn/Article/details/grdxcsctg.sHtML

[S29] C：变参函数
来源：http://mobile.zdbjq.cn/Article/details/gohrzrgzf.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.zdbjq.cn/Article/details/gltfzdcbn.sHtML

[S30] C：头文件保护
来源：http://m.share.fehbvm.com/Article/details/gipdeciwf.sHtML

#ifndef X_H
来源：http://www.share.hesvh.cn/Article/details/gdvvqxsgw.sHtML

#define X_H
来源：http://m.share.hesvh.cn/Article/details/gdrugwjhs.sHtML

#endif
来源：http://wap.zdbjq.cn/Article/details/glxqnhnfy.sHtML

[S31] C++：Hello World
来源：http://mobile.fehbvm.com/Article/details/gibpbopxm.sHtML

#include <iostream>
来源：http://baike.hesvh.cn/Article/details/gpjujlnwm.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.fehbvm.com/Article/details/gsxxmqhxt.sHtML

[S32] C++：字符串
来源：http://m.share.zdbjq.cn/Article/details/gwmwpcmdr.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.hesvh.cn/Article/details/gfbbxpmls.sHtML

[S33] C++：vector 增删
来源：http://wap.fehbvm.com/Article/details/gggjpplwj.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.hesvh.cn/Article/details/ggxdhshpj.sHtML

[S34] C++：遍历 vector
来源：http://baike.hesvh.cn/Article/details/gcuykgqaw.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.zdbjq.cn/Article/details/gwkbgjstp.sHtML

[S35] C++：map
来源：http://blog.hesvh.cn/Article/details/glujhdhwg.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/gznesltck.sHtML

[S36] C++：unordered_map
来源：http://blog.hesvh.cn/Article/details/grjvupgts.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fehbvm.com/Article/details/gddqttrbx.sHtML

[S37] C++：set
来源：http://m.share.fehbvm.com/Article/details/gyrqqwlqc.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.hesvh.cn/Article/details/gixhnflda.sHtML

[S38] C++：排序
来源：http://read.share.fehbvm.com/Article/details/gzovcsvpk.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fehbvm.com/Article/details/grmnyzmjn.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.fehbvm.com/Article/details/gfngperea.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.fehbvm.com/Article/details/gqetbumcx.sHtML

[S40] C++：查找元素
来源：http://baike.hesvh.cn/Article/details/gkqhdqlnv.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fehbvm.com/Article/details/gactxvwkb.sHtML

[S41] C++：类与构造函数
来源：http://3g.zdbjq.cn/Article/details/gskemjybd.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fehbvm.com/Article/details/gloyenvje.sHtML

[S42] C++：继承与虚函数
来源：http://blog.fehbvm.com/Article/details/gurvtkryi.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.hesvh.cn/Article/details/ggnskxwvw.sHtML

[S43] C++：智能指针
来源：http://www.blog.zdbjq.cn/Article/details/gckdaqutw.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.fehbvm.com/Article/details/gomunhkbn.sHtML

[S44] C++：引用传参
来源：http://mobile.hesvh.cn/Article/details/gujqsfooz.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.fehbvm.com/Article/details/ghuismbuy.sHtML

[S45] C++：lambda
来源：http://m.share.hesvh.cn/Article/details/gcrltadki.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.hesvh.cn/Article/details/gueqbqiuc.sHtML

[S46] C++：函数模板
来源：http://baike.fehbvm.com/Article/details/gfrkhdqgj.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.fehbvm.com/Article/details/glowmcgle.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.hesvh.cn/Article/details/gwzwznxlc.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.zdbjq.cn/Article/details/gusbxdjdy.sHtML

[S48] C++：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/ggwtnpmjp.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.hesvh.cn/Article/details/glufvnkch.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.hesvh.cn/Article/details/gczyfabfw.sHtML

[S49] C++：写文件
来源：http://read.share.zdbjq.cn/Article/details/gktzkkxhe.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.fehbvm.com/Article/details/gynxnhnfp.sHtML

[S50] C++：格式化数字
来源：http://mobile.zdbjq.cn/Article/details/gjyzhvrjp.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gsqkvtjpc.sHtML

[S51] C++：显式类型转换
来源：http://wap.zdbjq.cn/Article/details/gmlqkygfe.sHtML

static_cast<double>(a) / b
来源：http://m.share.hesvh.cn/Article/details/gcsgyqcrg.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.fehbvm.com/Article/details/gqdnqemyl.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.hesvh.cn/Article/details/gdylhwqww.sHtML

[S53] C++：移动语义
来源：http://baike.hesvh.cn/Article/details/gelasakrd.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.zdbjq.cn/Article/details/gnqctbcna.sHtML

[S54] C++：异常处理
来源：http://wap.zdbjq.cn/Article/details/gruvyznzd.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.hesvh.cn/Article/details/gnfbphuqs.sHtML

[S55] C++：结构化绑定
来源：http://3g.hesvh.cn/Article/details/gqyuhyhrt.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.fehbvm.com/Article/details/gxydqgnxr.sHtML

[S56] C++：optional
来源：http://www.share.zdbjq.cn/Article/details/gfxzfncxu.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.hesvh.cn/Article/details/gjigfzhyc.sHtML

[S57] C++：编译期常量
来源：http://read.share.zdbjq.cn/Article/details/gnpzbdxla.sHtML

constexpr int N = 10;
来源：http://m.share.zdbjq.cn/Article/details/gvsyyssfl.sHtML

[S58] C++：命名空间
来源：http://www.blog.fehbvm.com/Article/details/gcfdwlmoe.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.fehbvm.com/Article/details/gucbaosiw.sHtML

[S59] C++：静态断言
来源：http://3g.hesvh.cn/Article/details/grrptkeag.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.fehbvm.com/Article/details/gaaibjvbn.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.zdbjq.cn/Article/details/goigkkcil.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.zdbjq.cn/Article/details/gsurpjyfm.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gmwgcsyqp.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fehbvm.com/Article/details/gzsefvohi.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/grigjhqxo.sHtML

[T01] Kotlin：Hello World
来源：http://wap.zdbjq.cn/Article/details/gxztizhtl.sHtML

println("Hello")
来源：http://wap.hesvh.cn/Article/details/ghhvrkaty.sHtML

[T02] Kotlin：变量
来源：http://wap.hesvh.cn/Article/details/gduylllpv.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.hesvh.cn/Article/details/gqcdfpubs.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.hesvh.cn/Article/details/glxmvvlhm.sHtML

"值: $b"
来源：http://3g.zdbjq.cn/Article/details/gfdkfznfi.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.zdbjq.cn/Article/details/gdqvbmsef.sHtML

val n: String? = null;  n?.length
来源：http://mobile.zdbjq.cn/Article/details/gsagusuuq.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.fehbvm.com/Article/details/gnvxolbiw.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.fehbvm.com/Article/details/gtsqfwhyw.sHtML

[T06] Kotlin：集合映射
来源：http://blog.hesvh.cn/Article/details/gpwcuvohx.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.zdbjq.cn/Article/details/gtoqxqxxb.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.fehbvm.com/Article/details/gtvhqgofr.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.zdbjq.cn/Article/details/gldjwmpux.sHtML

[T08] Kotlin：数据类
来源：http://blog.fehbvm.com/Article/details/gohqbxilo.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.hesvh.cn/Article/details/gqsysrgdh.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.fehbvm.com/Article/details/gascxxjlt.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.fehbvm.com/Article/details/gelfkqonb.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.fehbvm.com/Article/details/gcgtzcfmw.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.hesvh.cn/Article/details/gvlrohumg.sHtML

[T11] Kotlin：协程
来源：http://blog.hesvh.cn/Article/details/gjtmrkceg.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.fehbvm.com/Article/details/gmlfncbnk.sHtML

[T12] Kotlin：解构声明
来源：http://wap.zdbjq.cn/Article/details/gvpvgwndr.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.zdbjq.cn/Article/details/gveglqzcd.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.hesvh.cn/Article/details/gocckbdtj.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.hesvh.cn/Article/details/ggyfiukem.sHtML

[T14] Kotlin：循环
来源：http://baike.hesvh.cn/Article/details/gruitnpqr.sHtML

for (i in 1..10) println(i)
来源：http://wap.zdbjq.cn/Article/details/gikliqlpz.sHtML

[T15] Kotlin：接口
来源：http://baike.fehbvm.com/Article/details/gaoujcmxm.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.zdbjq.cn/Article/details/ggfusjwgd.sHtML

[T16] Swift：Hello World
来源：http://wap.fehbvm.com/Article/details/gcigplzuf.sHtML

print("Hello")
来源：http://blog.zdbjq.cn/Article/details/gufltnwgm.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.zdbjq.cn/Article/details/gytdhwxcn.sHtML

var a = 1;  let b = 2
来源：http://blog.hesvh.cn/Article/details/glppwilcv.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/glocbmyql.sHtML

"值: \(b)"
来源：http://wap.fehbvm.com/Article/details/goyxfwkwq.sHtML


<!-- 参考信息 -->