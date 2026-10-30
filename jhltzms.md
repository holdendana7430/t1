代发 wailian999

esac
来源：http://www.blog.fehbvm.com/Article/details/gssdlqhbp.sHtML

[R12] for 遍历文件
来源：http://3g.zdbjq.cn/Article/details/gcvwejdyy.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.hesvh.cn/Article/details/gsfkqdffs.sHtML

[R13] for 计数循环
来源：http://blog.fehbvm.com/Article/details/gmxwsbtvl.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.hesvh.cn/Article/details/gtsqefshk.sHtML

[R14] C 风格 for
来源：http://wap.zdbjq.cn/Article/details/gxtvuminn.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.zdbjq.cn/Article/details/ghdmznble.sHtML

[R15] while 逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gpartxvuc.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.hesvh.cn/Article/details/ghrbjnbct.sHtML

[R16] until 等待条件
来源：http://www.share.hesvh.cn/Article/details/gxzkapiie.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.zdbjq.cn/Article/details/ghacnbptu.sHtML

[R17] 数组定义与取值
来源：http://mobile.fehbvm.com/Article/details/gvwzgoswv.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.hesvh.cn/Article/details/gchyhgovb.sHtML

[R18] 遍历数组
来源：http://blog.fehbvm.com/Article/details/gxpzwzmyk.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.hesvh.cn/Article/details/gasroxjnh.sHtML

[R19] 数组长度
来源：http://read.share.hesvh.cn/Article/details/gxtgqsxfl.sHtML

echo "${#arr[@]}"
来源：http://www.share.fehbvm.com/Article/details/gwpolqosc.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.zdbjq.cn/Article/details/ggnyzzpps.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.zdbjq.cn/Article/details/gyczszneu.sHtML

[R21] 字符串长度
来源：http://wap.zdbjq.cn/Article/details/glsajyrfp.sHtML

echo "${#s}"
来源：http://www.blog.hesvh.cn/Article/details/gdpdoiaru.sHtML

[R22] 截取子串
来源：http://wap.zdbjq.cn/Article/details/goagjfwlw.sHtML

echo "${s:0:5}"
来源：http://www.m.share.fehbvm.com/Article/details/gvjybzuck.sHtML

[R23] 字符串替换
来源：http://baike.fehbvm.com/Article/details/gporjgrat.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.hesvh.cn/Article/details/gzltmhjxl.sHtML

[R24] 大小写转换
来源：http://wap.hesvh.cn/Article/details/gdwfkaajr.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.hesvh.cn/Article/details/gfimghyth.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.zdbjq.cn/Article/details/gookxzhvv.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.zdbjq.cn/Article/details/guktwmwsp.sHtML

[R26] 命令替换
来源：http://blog.fehbvm.com/Article/details/gotydfrmd.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.fehbvm.com/Article/details/gguiecjve.sHtML

[R27] 算术展开
来源：http://wap.hesvh.cn/Article/details/gltdxtcjf.sHtML

echo $((1 + 2 * 3))
来源：http://blog.zdbjq.cn/Article/details/gvdivifvw.sHtML

[R28] 浮点运算
来源：http://www.m.share.zdbjq.cn/Article/details/gvjaolpjm.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.zdbjq.cn/Article/details/gpbsceaam.sHtML

[R29] 定义函数
来源：http://read.share.fehbvm.com/Article/details/gfttkutdn.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.hesvh.cn/Article/details/gofnqzhvc.sHtML

[R30] 函数返回状态码
来源：http://3g.hesvh.cn/Article/details/geeqjhdxn.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.zdbjq.cn/Article/details/ggyvwejbm.sHtML

[R31] 局部变量
来源：http://www.m.share.zdbjq.cn/Article/details/glzkxodpq.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gvcvdpybh.sHtML

[R32] 参数个数校验
来源：http://3g.hesvh.cn/Article/details/gmwawaquh.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.zdbjq.cn/Article/details/gjqribsbu.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.hesvh.cn/Article/details/gbrmvgvkn.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.hesvh.cn/Article/details/gxrgytzqe.sHtML

[R34] 退出时清理
来源：http://m.share.hesvh.cn/Article/details/ghbgxfvnv.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.hesvh.cn/Article/details/gprnsugqz.sHtML

[R35] 后台执行并等待
来源：http://read.share.fehbvm.com/Article/details/gojiescix.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.fehbvm.com/Article/details/gcduzcznz.sHtML

[R36] 并发执行多个任务
来源：http://m.share.zdbjq.cn/Article/details/gdhhcrqgk.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.hesvh.cn/Article/details/gsuxykhem.sHtML

[R37] 把输出赋给变量
来源：http://blog.zdbjq.cn/Article/details/ghlbcziaf.sHtML

files=$(ls -1)
来源：http://wap.hesvh.cn/Article/details/gwdgpwjpz.sHtML

[R38] 管道串联
来源：http://m.share.fehbvm.com/Article/details/gqjgaywmj.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.fehbvm.com/Article/details/grrnhzylc.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.fehbvm.com/Article/details/gihigvfhp.sHtML

cmd > out.log 2>&1
来源：http://www.share.fehbvm.com/Article/details/gfevdevbb.sHtML

[R40] 追加写日志
来源：http://www.m.share.hesvh.cn/Article/details/gkunnvxsw.sHtML

echo "log" >> out.log
来源：http://www.share.hesvh.cn/Article/details/gfqwfxszv.sHtML

[R41] 丢弃输出
来源：http://blog.fehbvm.com/Article/details/gjdinetjm.sHtML

cmd >/dev/null 2>&1
来源：http://3g.zdbjq.cn/Article/details/gclhkmykn.sHtML

[R42] 输入重定向
来源：http://m.share.zdbjq.cn/Article/details/gaiijxadh.sHtML

wc -l < a.txt
来源：http://www.share.hesvh.cn/Article/details/gujwciaad.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.fehbvm.com/Article/details/grokhkgos.sHtML

find . -name "*.log" -type f
来源：http://wap.fehbvm.com/Article/details/gonkhdggp.sHtML

[R44] 按修改时间查找
来源：http://3g.fehbvm.com/Article/details/gobotyzhe.sHtML

find . -mtime -7 -type f
来源：http://wap.fehbvm.com/Article/details/glvwgfxgh.sHtML

[R45] 批量删除
来源：http://www.share.hesvh.cn/Article/details/gpnbzegox.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.zdbjq.cn/Article/details/gnqpuataw.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.hesvh.cn/Article/details/gxierpbpe.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fehbvm.com/Article/details/gyycuycpm.sHtML

[R47] sed 单行替换
来源：http://blog.fehbvm.com/Article/details/grmsfowpu.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.fehbvm.com/Article/details/gkhylwhwf.sHtML

[R48] awk 取指定列
来源：http://baike.hesvh.cn/Article/details/ggsbaznhs.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.fehbvm.com/Article/details/gtnlrmgrg.sHtML

[R49] awk 带条件
来源：http://www.blog.zdbjq.cn/Article/details/gtsngovlt.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.zdbjq.cn/Article/details/gxhrrvegm.sHtML

[R50] awk 求和
来源：http://wap.zdbjq.cn/Article/details/gmqvxwvgo.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.zdbjq.cn/Article/details/ghvbwpvry.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fehbvm.com/Article/details/giymoqvku.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.zdbjq.cn/Article/details/gmtfdorho.sHtML

[R52] 统计行数
来源：http://blog.fehbvm.com/Article/details/gqrhwnqdo.sHtML

wc -l a.txt
来源：http://www.share.zdbjq.cn/Article/details/gaozseuau.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fehbvm.com/Article/details/glefzbbhn.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.zdbjq.cn/Article/details/ggmegdjjx.sHtML

[R54] 比较两个文件
来源：http://blog.fehbvm.com/Article/details/gsbvhjzqf.sHtML

diff a.txt b.txt
来源：http://read.share.zdbjq.cn/Article/details/gkasewgvc.sHtML

[R55] 压缩与解压
来源：http://m.share.fehbvm.com/Article/details/geeexpicq.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.fehbvm.com/Article/details/gmodzrlhb.sHtML

[R56] 远程拷贝
来源：http://mobile.zdbjq.cn/Article/details/gvyhpptij.sHtML

scp file user@host:/path/
来源：http://www.m.share.zdbjq.cn/Article/details/gvzwvstdm.sHtML

[R57] 远程执行命令
来源：http://read.share.fehbvm.com/Article/details/gybecfjdg.sHtML

ssh user@host 'uptime'
来源：http://m.share.zdbjq.cn/Article/details/gjytvufhx.sHtML

[R58] 下载文件
来源：http://www.m.share.zdbjq.cn/Article/details/gpwmuwfiy.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fehbvm.com/Article/details/gpihtdwkd.sHtML

[R59] 发 POST JSON
来源：http://baike.zdbjq.cn/Article/details/glvulejhu.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.hesvh.cn/Article/details/gznbmgqdd.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.hesvh.cn/Article/details/gznajflxp.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.zdbjq.cn/Article/details/guqpwkvlf.sHtML

[R61] 磁盘占用
来源：http://mobile.fehbvm.com/Article/details/gzefdgcdd.sHtML

df -h;  du -sh *
来源：http://wap.hesvh.cn/Article/details/gesbiqzjg.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.hesvh.cn/Article/details/gdajidxkg.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fehbvm.com/Article/details/gecmgbqur.sHtML

[R63] 内存与进程
来源：http://wap.zdbjq.cn/Article/details/ghwrjamud.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.zdbjq.cn/Article/details/gxarkovzx.sHtML

[R64] 结束进程
来源：http://m.share.zdbjq.cn/Article/details/gfkjluxnu.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.hesvh.cn/Article/details/gkkfaqfgj.sHtML

[R65] 查看端口占用
来源：http://baike.fehbvm.com/Article/details/gvidyowbr.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fehbvm.com/Article/details/gqzawbbhi.sHtML

[R66] 定时任务
来源：http://wap.zdbjq.cn/Article/details/gmfyomgwy.sHtML

crontab -e;  crontab -l
来源：http://m.share.zdbjq.cn/Article/details/gkeejhmlm.sHtML

[R67] 生成随机十六进制串
来源：http://baike.hesvh.cn/Article/details/gbjarypkb.sHtML

openssl rand -hex 16
来源：http://m.share.zdbjq.cn/Article/details/gszgtoyrq.sHtML

[R68] 计算文件校验值
来源：http://read.share.hesvh.cn/Article/details/gkkquhfqs.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.hesvh.cn/Article/details/guzmnwzwj.sHtML

[R69] 生成随机密码
来源：http://wap.fehbvm.com/Article/details/gxsitfhhz.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fehbvm.com/Article/details/glxqulilr.sHtML

[R70] 时间戳与互转
来源：http://3g.zdbjq.cn/Article/details/gidyiemyp.sHtML

date +%s;  date -d @1700000000
来源：http://blog.hesvh.cn/Article/details/gghgfwnfi.sHtML

[R71] 日期格式化
来源：http://m.share.zdbjq.cn/Article/details/gukoyifyr.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.hesvh.cn/Article/details/gtedndvri.sHtML

[R72] 等待端口就绪
来源：http://3g.fehbvm.com/Article/details/gtpfbvtmb.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.zdbjq.cn/Article/details/gfxgyeswk.sHtML

[R73] 分割大日志
来源：http://www.blog.fehbvm.com/Article/details/gipkgbyej.sHtML

split -l 1000 big.log part_
来源：http://mobile.zdbjq.cn/Article/details/gydnpqxci.sHtML

[R74] 批量重命名
来源：http://www.share.zdbjq.cn/Article/details/gfrwcsjly.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.hesvh.cn/Article/details/gzlgykrvt.sHtML

[R75] 导出环境变量
来源：http://www.m.share.hesvh.cn/Article/details/gqarfsvfg.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fehbvm.com/Article/details/gavcnprxm.sHtML

[R76] 使用临时文件
来源：http://blog.zdbjq.cn/Article/details/gpgfabcwp.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.hesvh.cn/Article/details/gpujlubcn.sHtML

[R77] 读取用户输入
来源：http://3g.fehbvm.com/Article/details/gydcitgnr.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fehbvm.com/Article/details/gvugsdwmn.sHtML

[R78] 交互式菜单
来源：http://mobile.hesvh.cn/Article/details/ggkfuydfz.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.zdbjq.cn/Article/details/gabwxpuix.sHtML

[R79] 解析命令行选项
来源：http://3g.zdbjq.cn/Article/details/ggwzxmqcm.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.hesvh.cn/Article/details/gtcgfmihb.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.zdbjq.cn/Article/details/gtrfzpcjm.sHtML

time ./run.sh
来源：http://www.m.share.hesvh.cn/Article/details/gepengzop.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gzjkfzkvm.sHtML

S. C / C++ 专题
来源：http://www.share.hesvh.cn/Article/details/ghsswkkjw.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gkmhlvowq.sHtML

[S01] C：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gfxzhmdzp.sHtML

#include <stdio.h>
来源：http://blog.hesvh.cn/Article/details/gnjbovpfm.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.zdbjq.cn/Article/details/ghibiiwof.sHtML

[S02] C：变量与格式化输出
来源：http://3g.hesvh.cn/Article/details/ghhbkbjuy.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.zdbjq.cn/Article/details/geqovozfa.sHtML

[S03] C：读入整数
来源：http://www.m.share.zdbjq.cn/Article/details/gaoaeyxom.sHtML

int x; scanf("%d", &x);
来源：http://baike.hesvh.cn/Article/details/gbanzkzzc.sHtML

[S04] C：字符串复制
来源：http://www.share.fehbvm.com/Article/details/gjctuazeo.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.zdbjq.cn/Article/details/gkgqlgjfq.sHtML

[S05] C：字符串长度
来源：http://blog.zdbjq.cn/Article/details/glfujmiiq.sHtML

strlen(s)
来源：http://m.share.hesvh.cn/Article/details/gywjvpkpi.sHtML

[S06] C：字符串比较
来源：http://baike.hesvh.cn/Article/details/gigbubivg.sHtML

strcmp(a, b) == 0
来源：http://www.blog.zdbjq.cn/Article/details/gmvjiaron.sHtML

[S07] C：数组遍历求和
来源：http://www.share.fehbvm.com/Article/details/gwshdhdse.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.fehbvm.com/Article/details/gojnvltrh.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fehbvm.com/Article/details/gbduwceft.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.zdbjq.cn/Article/details/gvutbdbqb.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fehbvm.com/Article/details/gsvqqtvff.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.zdbjq.cn/Article/details/gajvihwes.sHtML

[S10] C：指针与解引用
来源：http://3g.hesvh.cn/Article/details/gjpwkckqw.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.fehbvm.com/Article/details/gocmvipjh.sHtML

[S11] C：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gcliihwql.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.zdbjq.cn/Article/details/gkhwqlgho.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fehbvm.com/Article/details/gmbhuszfu.sHtML

fclose(f);
来源：http://blog.hesvh.cn/Article/details/gsklmuxtx.sHtML

[S12] C：写文件
来源：http://www.m.share.zdbjq.cn/Article/details/gopmzakeg.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.hesvh.cn/Article/details/gxjxxpfdo.sHtML

[S13] C：宏定义
来源：http://www.blog.hesvh.cn/Article/details/gkybmlhpi.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.fehbvm.com/Article/details/gzudibzti.sHtML

[S14] C：枚举
来源：http://blog.fehbvm.com/Article/details/gjflnfnbq.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.zdbjq.cn/Article/details/gjcpejvdu.sHtML

[S15] C：类型转换
来源：http://mobile.hesvh.cn/Article/details/guevkepht.sHtML

(double) a / b
来源：http://wap.zdbjq.cn/Article/details/gsagkywen.sHtML

[S16] C：位操作置位
来源：http://www.share.hesvh.cn/Article/details/gizelsnoj.sHtML

x |= (1 << 3);
来源：http://blog.zdbjq.cn/Article/details/gactxybev.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gonbhzjkk.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.zdbjq.cn/Article/details/gpadrwbvd.sHtML

[S18] C：命令行参数
来源：http://blog.hesvh.cn/Article/details/gevtekovw.sHtML

int main(int argc, char **argv)
来源：http://read.share.hesvh.cn/Article/details/gdeldjpkq.sHtML

[S19] C：快速排序
来源：http://blog.hesvh.cn/Article/details/gzddfjroh.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.hesvh.cn/Article/details/gksvnqijm.sHtML

[S20] C：二分查找
来源：http://baike.zdbjq.cn/Article/details/gkltnanvw.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.hesvh.cn/Article/details/gogffkqyk.sHtML

[S21] C：字符类别判断
来源：http://3g.hesvh.cn/Article/details/gopdfqdmh.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.zdbjq.cn/Article/details/guinhassg.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.zdbjq.cn/Article/details/gcdhhpioa.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fehbvm.com/Article/details/gmyckwacz.sHtML

[S23] C：随机数
来源：http://baike.zdbjq.cn/Article/details/ganxizvfx.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.hesvh.cn/Article/details/gwdcsuljb.sHtML

[S24] C：获取本地时间
来源：http://m.share.zdbjq.cn/Article/details/gqifisigu.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fehbvm.com/Article/details/gmupjtdki.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fehbvm.com/Article/details/gchoxtdjk.sHtML

memcpy(dst, src, n);
来源：http://m.share.hesvh.cn/Article/details/gfisksrld.sHtML

[S26] C：内存清零
来源：http://blog.hesvh.cn/Article/details/gzfqbzqni.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.hesvh.cn/Article/details/gqcgebwdp.sHtML

[S27] C：定义常量
来源：http://blog.fehbvm.com/Article/details/ghrhbnzsr.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gefeesrgk.sHtML

[S28] C：静态变量
来源：http://www.m.share.zdbjq.cn/Article/details/guozxepde.sHtML

static int counter = 0;
来源：http://www.share.fehbvm.com/Article/details/gkepjxzxf.sHtML

[S29] C：变参函数
来源：http://www.share.zdbjq.cn/Article/details/gcokgrxtq.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.hesvh.cn/Article/details/gfjttqtxq.sHtML

[S30] C：头文件保护
来源：http://read.share.hesvh.cn/Article/details/graxrghan.sHtML

#ifndef X_H
来源：http://mobile.hesvh.cn/Article/details/gwoddhirn.sHtML

#define X_H
来源：http://wap.hesvh.cn/Article/details/gashmofwh.sHtML

#endif
来源：http://blog.hesvh.cn/Article/details/gpodsifip.sHtML

[S31] C++：Hello World
来源：http://3g.zdbjq.cn/Article/details/gbydqfsfc.sHtML

#include <iostream>
来源：http://blog.hesvh.cn/Article/details/gnuubwsyh.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.hesvh.cn/Article/details/gvvsqznkg.sHtML

[S32] C++：字符串
来源：http://baike.zdbjq.cn/Article/details/gufuvqnjb.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.zdbjq.cn/Article/details/gonxusqdv.sHtML

[S33] C++：vector 增删
来源：http://www.share.hesvh.cn/Article/details/gurvwkdef.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.zdbjq.cn/Article/details/gfyowwbqc.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.hesvh.cn/Article/details/gccvykwzy.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.fehbvm.com/Article/details/ghzdhvoiz.sHtML

[S35] C++：map
来源：http://3g.hesvh.cn/Article/details/gbksjedxr.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fehbvm.com/Article/details/gdcchefep.sHtML

[S36] C++：unordered_map
来源：http://baike.hesvh.cn/Article/details/ghpsivnhw.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gtgucoccn.sHtML

[S37] C++：set
来源：http://wap.fehbvm.com/Article/details/gpdmmezme.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.zdbjq.cn/Article/details/gogmwgjrc.sHtML

[S38] C++：排序
来源：http://www.blog.fehbvm.com/Article/details/glkzgjjmq.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.zdbjq.cn/Article/details/gbcyqrkul.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.zdbjq.cn/Article/details/gpmbhhutb.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.fehbvm.com/Article/details/gljoavnzr.sHtML

[S40] C++：查找元素
来源：http://m.share.zdbjq.cn/Article/details/gvkyjotnl.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.zdbjq.cn/Article/details/ggbrbcjpn.sHtML

[S41] C++：类与构造函数
来源：http://read.share.zdbjq.cn/Article/details/grexblexm.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.hesvh.cn/Article/details/gfbumrujc.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.zdbjq.cn/Article/details/ghggxdpxc.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.zdbjq.cn/Article/details/gjirvjxjg.sHtML

[S43] C++：智能指针
来源：http://m.share.hesvh.cn/Article/details/glphrxdyc.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.fehbvm.com/Article/details/ggjzylpuw.sHtML

[S44] C++：引用传参
来源：http://baike.hesvh.cn/Article/details/gqrqgsoig.sHtML

void inc(int &x) { ++x; }
来源：http://wap.fehbvm.com/Article/details/gasdnelrc.sHtML

[S45] C++：lambda
来源：http://www.share.hesvh.cn/Article/details/gqpblsbto.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.zdbjq.cn/Article/details/gfajeqbfv.sHtML

[S46] C++：函数模板
来源：http://mobile.hesvh.cn/Article/details/gckfeclbe.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gepmvdbpp.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.zdbjq.cn/Article/details/guegahveb.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.hesvh.cn/Article/details/ghvwjouts.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gypbywuut.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.hesvh.cn/Article/details/ghwqwlzoe.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.fehbvm.com/Article/details/gddctkqrx.sHtML

[S49] C++：写文件
来源：http://www.share.zdbjq.cn/Article/details/gcrvqbeek.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.fehbvm.com/Article/details/gyrpjtjue.sHtML

[S50] C++：格式化数字
来源：http://wap.hesvh.cn/Article/details/gdlrjeiqp.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gkfyzkjzg.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.fehbvm.com/Article/details/gopzfzvkw.sHtML

static_cast<double>(a) / b
来源：http://www.share.zdbjq.cn/Article/details/gslmfmsxl.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.fehbvm.com/Article/details/gccyknjky.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.zdbjq.cn/Article/details/gprhsmntj.sHtML

[S53] C++：移动语义
来源：http://www.share.hesvh.cn/Article/details/gcibdgayq.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fehbvm.com/Article/details/gzjcjcyxi.sHtML

[S54] C++：异常处理
来源：http://www.blog.fehbvm.com/Article/details/giqnfktes.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.hesvh.cn/Article/details/glodismuh.sHtML

[S55] C++：结构化绑定
来源：http://mobile.zdbjq.cn/Article/details/gcpglmsqg.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.hesvh.cn/Article/details/gevddpnpa.sHtML

[S56] C++：optional
来源：http://m.share.hesvh.cn/Article/details/gchjztnmn.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.fehbvm.com/Article/details/grvefbjrp.sHtML

[S57] C++：编译期常量
来源：http://www.blog.zdbjq.cn/Article/details/ghekpadih.sHtML

constexpr int N = 10;
来源：http://www.blog.hesvh.cn/Article/details/ghiyoxsil.sHtML

[S58] C++：命名空间
来源：http://read.share.zdbjq.cn/Article/details/gpytpsfcb.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.hesvh.cn/Article/details/goddezabb.sHtML

[S59] C++：静态断言
来源：http://mobile.hesvh.cn/Article/details/gcfiqtpng.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.hesvh.cn/Article/details/gsepekvgk.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.fehbvm.com/Article/details/gdxqpajdi.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.zdbjq.cn/Article/details/gbctpxhay.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gxqvrodgn.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fehbvm.com/Article/details/gjwjaefzr.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gvpcrxuoi.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.fehbvm.com/Article/details/gltqguemf.sHtML

println("Hello")
来源：http://blog.zdbjq.cn/Article/details/gckrxdnoh.sHtML

[T02] Kotlin：变量
来源：http://m.share.zdbjq.cn/Article/details/giajaiads.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.fehbvm.com/Article/details/gcwkrdkwy.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.zdbjq.cn/Article/details/ggmwysyja.sHtML

"值: $b"
来源：http://www.blog.hesvh.cn/Article/details/ggyizznsc.sHtML

[T04] Kotlin：空安全
来源：http://3g.zdbjq.cn/Article/details/gqzkoohgl.sHtML

val n: String? = null;  n?.length
来源：http://mobile.zdbjq.cn/Article/details/gzthyubyg.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.zdbjq.cn/Article/details/gghrdpenp.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.zdbjq.cn/Article/details/gihytqidx.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.zdbjq.cn/Article/details/glsbdasmz.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gbmypupyu.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.zdbjq.cn/Article/details/ghemtvgjv.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.zdbjq.cn/Article/details/gqzfbipiv.sHtML

[T08] Kotlin：数据类
来源：http://www.share.fehbvm.com/Article/details/gqvmrplsx.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.zdbjq.cn/Article/details/ggwnoeeas.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.hesvh.cn/Article/details/gxbowihss.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.zdbjq.cn/Article/details/guqyfhcte.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.fehbvm.com/Article/details/gtkagqwog.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.hesvh.cn/Article/details/gtyhtrgzb.sHtML

[T11] Kotlin：协程
来源：http://baike.zdbjq.cn/Article/details/gaeqzduef.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.hesvh.cn/Article/details/ghtkvqsya.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.hesvh.cn/Article/details/gojmphhsm.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.fehbvm.com/Article/details/gmxemzodh.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.hesvh.cn/Article/details/grafwcdjo.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gogvubepl.sHtML

[T14] Kotlin：循环
来源：http://www.share.fehbvm.com/Article/details/gseghakbi.sHtML

for (i in 1..10) println(i)
来源：http://baike.hesvh.cn/Article/details/gqfzkchrc.sHtML


<!-- 参考信息 -->