代发 wailian999

case "$1" in
来源：http://read.share.zdbjq.cn/Article/details/geuhprdyq.sHtML

start) echo "启动" ;;
来源：http://read.share.fehbvm.com/Article/details/gffntujhr.sHtML

stop)  echo "停止" ;;
来源：http://wap.zdbjq.cn/Article/details/gkrwogqlx.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.fehbvm.com/Article/details/gmnyxkdzs.sHtML

esac
来源：http://mobile.hesvh.cn/Article/details/godmwqzhu.sHtML

[R12] for 遍历文件
来源：http://www.m.share.hesvh.cn/Article/details/gmldtcegv.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.hesvh.cn/Article/details/grhclwiel.sHtML

[R13] for 计数循环
来源：http://www.blog.fehbvm.com/Article/details/gkkcovzvl.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.fehbvm.com/Article/details/gegqefgjj.sHtML

[R14] C 风格 for
来源：http://mobile.hesvh.cn/Article/details/gdokvfpgj.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.hesvh.cn/Article/details/giglqwtuu.sHtML

[R15] while 逐行读文件
来源：http://wap.hesvh.cn/Article/details/gzxmrpckq.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.hesvh.cn/Article/details/gpmopuxcl.sHtML

[R16] until 等待条件
来源：http://www.blog.zdbjq.cn/Article/details/gczohxdyn.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.fehbvm.com/Article/details/gremtmubk.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.fehbvm.com/Article/details/gzvbvxpce.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.zdbjq.cn/Article/details/gflvzbavj.sHtML

[R18] 遍历数组
来源：http://baike.zdbjq.cn/Article/details/gedzefrib.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.hesvh.cn/Article/details/ghtfltbkj.sHtML

[R19] 数组长度
来源：http://wap.hesvh.cn/Article/details/gzqgohusg.sHtML

echo "${#arr[@]}"
来源：http://mobile.zdbjq.cn/Article/details/ghanxxgdf.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.zdbjq.cn/Article/details/gdhyztatr.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.hesvh.cn/Article/details/gwmkachvf.sHtML

[R21] 字符串长度
来源：http://m.share.fehbvm.com/Article/details/gjhaarjdi.sHtML

echo "${#s}"
来源：http://mobile.hesvh.cn/Article/details/gsoyolwrf.sHtML

[R22] 截取子串
来源：http://wap.hesvh.cn/Article/details/gyedqhzvi.sHtML

echo "${s:0:5}"
来源：http://baike.fehbvm.com/Article/details/gjrconfdn.sHtML

[R23] 字符串替换
来源：http://www.m.share.fehbvm.com/Article/details/gwyattmxa.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.fehbvm.com/Article/details/glrgiufvs.sHtML

[R24] 大小写转换
来源：http://mobile.zdbjq.cn/Article/details/gqzonzqlk.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.fehbvm.com/Article/details/gmmgapjnv.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.fehbvm.com/Article/details/gwivjlqzn.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fehbvm.com/Article/details/gthbmvxql.sHtML

[R26] 命令替换
来源：http://3g.fehbvm.com/Article/details/gusrwwrdz.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.hesvh.cn/Article/details/gfsrackqa.sHtML

[R27] 算术展开
来源：http://blog.zdbjq.cn/Article/details/gjbwwxeqh.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.hesvh.cn/Article/details/gvktncxxf.sHtML

[R28] 浮点运算
来源：http://www.m.share.hesvh.cn/Article/details/gyfuivtea.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.zdbjq.cn/Article/details/gqxxsrium.sHtML

[R29] 定义函数
来源：http://mobile.fehbvm.com/Article/details/gdowcbmyk.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.zdbjq.cn/Article/details/gdrwziwoa.sHtML

[R30] 函数返回状态码
来源：http://3g.fehbvm.com/Article/details/gtwrcunpr.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.fehbvm.com/Article/details/gqlzqyhdh.sHtML

[R31] 局部变量
来源：http://www.share.hesvh.cn/Article/details/giefxdicc.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fehbvm.com/Article/details/gidletcpl.sHtML

[R32] 参数个数校验
来源：http://mobile.zdbjq.cn/Article/details/gwchsxcpq.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.fehbvm.com/Article/details/gquoifwgc.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.hesvh.cn/Article/details/gnqoqaitl.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.fehbvm.com/Article/details/goioczipy.sHtML

[R34] 退出时清理
来源：http://baike.fehbvm.com/Article/details/gdjpiyarc.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fehbvm.com/Article/details/gbzsmtglq.sHtML

[R35] 后台执行并等待
来源：http://m.share.fehbvm.com/Article/details/glhduoxci.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.hesvh.cn/Article/details/glajdjczf.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.zdbjq.cn/Article/details/gouvcqbum.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.zdbjq.cn/Article/details/givmiyvaw.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.zdbjq.cn/Article/details/gpculokik.sHtML

files=$(ls -1)
来源：http://wap.fehbvm.com/Article/details/guaeoaxje.sHtML

[R38] 管道串联
来源：http://wap.zdbjq.cn/Article/details/giretrosa.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.hesvh.cn/Article/details/gxvifsail.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.zdbjq.cn/Article/details/grtzarvlg.sHtML

cmd > out.log 2>&1
来源：http://www.share.zdbjq.cn/Article/details/gbbqrecog.sHtML

[R40] 追加写日志
来源：http://blog.hesvh.cn/Article/details/gblxkzirr.sHtML

echo "log" >> out.log
来源：http://3g.zdbjq.cn/Article/details/gbzjohbho.sHtML

[R41] 丢弃输出
来源：http://www.m.share.zdbjq.cn/Article/details/gwbgjwafa.sHtML

cmd >/dev/null 2>&1
来源：http://baike.zdbjq.cn/Article/details/gbqvooivo.sHtML

[R42] 输入重定向
来源：http://3g.hesvh.cn/Article/details/gvgqyswli.sHtML

wc -l < a.txt
来源：http://mobile.hesvh.cn/Article/details/gjyyubely.sHtML

[R43] 按名字查找文件
来源：http://www.share.hesvh.cn/Article/details/grdaphpan.sHtML

find . -name "*.log" -type f
来源：http://read.share.zdbjq.cn/Article/details/goordhqyr.sHtML

[R44] 按修改时间查找
来源：http://baike.hesvh.cn/Article/details/gpabzzfwb.sHtML

find . -mtime -7 -type f
来源：http://www.share.zdbjq.cn/Article/details/gpxwibpza.sHtML

[R45] 批量删除
来源：http://m.share.zdbjq.cn/Article/details/gczjzbwvt.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.zdbjq.cn/Article/details/gkdvesfdu.sHtML

[R46] 递归替换文件内容
来源：http://m.share.hesvh.cn/Article/details/gxagbispb.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.zdbjq.cn/Article/details/gqjnyazyg.sHtML

[R47] sed 单行替换
来源：http://blog.zdbjq.cn/Article/details/gszccobdz.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/ggtdfiagq.sHtML

[R48] awk 取指定列
来源：http://mobile.zdbjq.cn/Article/details/gszsnuawv.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.fehbvm.com/Article/details/gwpjkuwuz.sHtML

[R49] awk 带条件
来源：http://www.blog.zdbjq.cn/Article/details/gmiyjrrqe.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.fehbvm.com/Article/details/gnfwttasq.sHtML

[R50] awk 求和
来源：http://baike.hesvh.cn/Article/details/gwjwyqlgm.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fehbvm.com/Article/details/ggapdyqfr.sHtML

[R51] 排序去重取前几
来源：http://www.share.zdbjq.cn/Article/details/gxdeeudjb.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.hesvh.cn/Article/details/gbsgqxfip.sHtML

[R52] 统计行数
来源：http://m.share.fehbvm.com/Article/details/gpjimpkzw.sHtML

wc -l a.txt
来源：http://www.share.zdbjq.cn/Article/details/gsuhhtklg.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.zdbjq.cn/Article/details/goebwlbqm.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.zdbjq.cn/Article/details/gtufejeum.sHtML

[R54] 比较两个文件
来源：http://mobile.fehbvm.com/Article/details/gpbqoyoen.sHtML

diff a.txt b.txt
来源：http://baike.fehbvm.com/Article/details/gszdjlbac.sHtML

[R55] 压缩与解压
来源：http://wap.hesvh.cn/Article/details/gwpzavyyj.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.zdbjq.cn/Article/details/gnliqwolv.sHtML

[R56] 远程拷贝
来源：http://blog.hesvh.cn/Article/details/gyzxwtsqo.sHtML

scp file user@host:/path/
来源：http://www.blog.zdbjq.cn/Article/details/gifbdtdhc.sHtML

[R57] 远程执行命令
来源：http://m.share.fehbvm.com/Article/details/gmojivmes.sHtML

ssh user@host 'uptime'
来源：http://3g.zdbjq.cn/Article/details/gtabjjdyo.sHtML

[R58] 下载文件
来源：http://3g.hesvh.cn/Article/details/gwcxrvtop.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.fehbvm.com/Article/details/ggxtinxqg.sHtML

[R59] 发 POST JSON
来源：http://www.share.fehbvm.com/Article/details/geyaymaay.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fehbvm.com/Article/details/gnxfpyjju.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.fehbvm.com/Article/details/grisoaykb.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fehbvm.com/Article/details/gbwurzugv.sHtML

[R61] 磁盘占用
来源：http://3g.hesvh.cn/Article/details/ghndaswyc.sHtML

df -h;  du -sh *
来源：http://www.m.share.hesvh.cn/Article/details/gdjhezwpq.sHtML

[R62] 找最占空间的文件
来源：http://m.share.hesvh.cn/Article/details/gyknfpikv.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.hesvh.cn/Article/details/gyppnzvyt.sHtML

[R63] 内存与进程
来源：http://www.share.fehbvm.com/Article/details/gvrfnwvdk.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.zdbjq.cn/Article/details/ghtvqdnbu.sHtML

[R64] 结束进程
来源：http://baike.fehbvm.com/Article/details/grtyaqfhv.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.hesvh.cn/Article/details/ggunymzrg.sHtML

[R65] 查看端口占用
来源：http://wap.hesvh.cn/Article/details/gobfupftv.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.zdbjq.cn/Article/details/gojsuxjnr.sHtML

[R66] 定时任务
来源：http://m.share.fehbvm.com/Article/details/giyjgddlx.sHtML

crontab -e;  crontab -l
来源：http://mobile.zdbjq.cn/Article/details/ggacuiydu.sHtML

[R67] 生成随机十六进制串
来源：http://wap.zdbjq.cn/Article/details/gdazyipgl.sHtML

openssl rand -hex 16
来源：http://read.share.fehbvm.com/Article/details/gvbotyiat.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.hesvh.cn/Article/details/gmxlvftou.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.hesvh.cn/Article/details/givacjdxr.sHtML

[R69] 生成随机密码
来源：http://mobile.hesvh.cn/Article/details/gjrpmurin.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.zdbjq.cn/Article/details/gkkpysihx.sHtML

[R70] 时间戳与互转
来源：http://www.share.hesvh.cn/Article/details/gohyieuqo.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.hesvh.cn/Article/details/gflptywty.sHtML

[R71] 日期格式化
来源：http://blog.hesvh.cn/Article/details/gblkvzccr.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.hesvh.cn/Article/details/gvrgzyiok.sHtML

[R72] 等待端口就绪
来源：http://mobile.zdbjq.cn/Article/details/glonioalz.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.hesvh.cn/Article/details/gsvwtmquj.sHtML

[R73] 分割大日志
来源：http://mobile.zdbjq.cn/Article/details/gxshhlggl.sHtML

split -l 1000 big.log part_
来源：http://www.blog.hesvh.cn/Article/details/glbmugslj.sHtML

[R74] 批量重命名
来源：http://blog.fehbvm.com/Article/details/gsjjggaih.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.zdbjq.cn/Article/details/gbzjhghxc.sHtML

[R75] 导出环境变量
来源：http://blog.hesvh.cn/Article/details/gcvpudkwv.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.hesvh.cn/Article/details/gobiquljz.sHtML

[R76] 使用临时文件
来源：http://m.share.fehbvm.com/Article/details/gmajupzoj.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.zdbjq.cn/Article/details/guzdffgen.sHtML

[R77] 读取用户输入
来源：http://mobile.fehbvm.com/Article/details/gywmhndxm.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fehbvm.com/Article/details/gephuvxfq.sHtML

[R78] 交互式菜单
来源：http://m.share.zdbjq.cn/Article/details/gnmjkcytl.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.hesvh.cn/Article/details/gqydkqnkk.sHtML

[R79] 解析命令行选项
来源：http://blog.fehbvm.com/Article/details/gkuucgvpg.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fehbvm.com/Article/details/godyqkgct.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.fehbvm.com/Article/details/gghcoabgf.sHtML

time ./run.sh
来源：http://baike.zdbjq.cn/Article/details/gohwwyvnm.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gubvezrvw.sHtML

S. C / C++ 专题
来源：http://blog.fehbvm.com/Article/details/ggjyaelat.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gtqksmeex.sHtML

[S01] C：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gvmtnazfp.sHtML

#include <stdio.h>
来源：http://wap.zdbjq.cn/Article/details/gkpgphtee.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.hesvh.cn/Article/details/gmtmsdcmy.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.hesvh.cn/Article/details/gxarfgdss.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.fehbvm.com/Article/details/gtpritjxe.sHtML

[S03] C：读入整数
来源：http://www.share.zdbjq.cn/Article/details/gohldpiqp.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.zdbjq.cn/Article/details/ghrobmthz.sHtML

[S04] C：字符串复制
来源：http://3g.hesvh.cn/Article/details/gkosbtvst.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.zdbjq.cn/Article/details/gfizkcpsn.sHtML

[S05] C：字符串长度
来源：http://blog.zdbjq.cn/Article/details/gtpgjlcuz.sHtML

strlen(s)
来源：http://m.share.hesvh.cn/Article/details/grhvxdfgt.sHtML

[S06] C：字符串比较
来源：http://blog.zdbjq.cn/Article/details/gycjokwkj.sHtML

strcmp(a, b) == 0
来源：http://baike.hesvh.cn/Article/details/gxlpdabpe.sHtML

[S07] C：数组遍历求和
来源：http://baike.hesvh.cn/Article/details/giublyexc.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.hesvh.cn/Article/details/gfrjubywe.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.zdbjq.cn/Article/details/gpbdkhvqt.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.hesvh.cn/Article/details/gkielkubw.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.zdbjq.cn/Article/details/gocmbzlkg.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.hesvh.cn/Article/details/gxwssajvw.sHtML

[S10] C：指针与解引用
来源：http://mobile.fehbvm.com/Article/details/gkbjxakrn.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fehbvm.com/Article/details/gtwhtobir.sHtML

[S11] C：逐行读文件
来源：http://3g.fehbvm.com/Article/details/geongtjek.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fehbvm.com/Article/details/guklnnyou.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.hesvh.cn/Article/details/gutlltewc.sHtML

fclose(f);
来源：http://www.share.fehbvm.com/Article/details/ghclkigws.sHtML

[S12] C：写文件
来源：http://wap.zdbjq.cn/Article/details/glndepyjf.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.hesvh.cn/Article/details/gnjxplrtd.sHtML

[S13] C：宏定义
来源：http://baike.hesvh.cn/Article/details/gfhfcodiv.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.hesvh.cn/Article/details/grdavnrjf.sHtML

[S14] C：枚举
来源：http://www.share.zdbjq.cn/Article/details/gkfbbhvdu.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.zdbjq.cn/Article/details/gkqunicjm.sHtML

[S15] C：类型转换
来源：http://mobile.hesvh.cn/Article/details/gvdngbhjy.sHtML

(double) a / b
来源：http://www.blog.fehbvm.com/Article/details/gjwnlzswz.sHtML

[S16] C：位操作置位
来源：http://www.blog.zdbjq.cn/Article/details/goltxpyty.sHtML

x |= (1 << 3);
来源：http://www.m.share.fehbvm.com/Article/details/glcvdbddk.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.fehbvm.com/Article/details/gsnwbwhdh.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.hesvh.cn/Article/details/gtblusbof.sHtML

[S18] C：命令行参数
来源：http://blog.hesvh.cn/Article/details/gqjchwwnv.sHtML

int main(int argc, char **argv)
来源：http://read.share.zdbjq.cn/Article/details/ghmzehvac.sHtML

[S19] C：快速排序
来源：http://wap.zdbjq.cn/Article/details/gjcftohvf.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.hesvh.cn/Article/details/gxivfekll.sHtML

[S20] C：二分查找
来源：http://www.m.share.hesvh.cn/Article/details/gbjjclvwk.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.zdbjq.cn/Article/details/gubokpzsn.sHtML

[S21] C：字符类别判断
来源：http://www.blog.hesvh.cn/Article/details/gqrszxktl.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.zdbjq.cn/Article/details/gkikirjyj.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.hesvh.cn/Article/details/ghiatmmpg.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.hesvh.cn/Article/details/gycsggpwg.sHtML

[S23] C：随机数
来源：http://mobile.zdbjq.cn/Article/details/gxotaisut.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.hesvh.cn/Article/details/gmmnjvjcu.sHtML

[S24] C：获取本地时间
来源：http://www.blog.hesvh.cn/Article/details/guhuciywc.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.hesvh.cn/Article/details/gflxkfjwg.sHtML

[S25] C：内存拷贝
来源：http://blog.zdbjq.cn/Article/details/gvvkvchmt.sHtML

memcpy(dst, src, n);
来源：http://3g.hesvh.cn/Article/details/gobbadizj.sHtML

[S26] C：内存清零
来源：http://m.share.zdbjq.cn/Article/details/gyoedmcdf.sHtML

memset(a, 0, sizeof a);
来源：http://blog.hesvh.cn/Article/details/gvgjjhluw.sHtML

[S27] C：定义常量
来源：http://m.share.fehbvm.com/Article/details/gowueicmf.sHtML

const double PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gmpofdxkj.sHtML

[S28] C：静态变量
来源：http://mobile.hesvh.cn/Article/details/gfcjifjnn.sHtML

static int counter = 0;
来源：http://blog.fehbvm.com/Article/details/gwfvabntr.sHtML

[S29] C：变参函数
来源：http://www.share.hesvh.cn/Article/details/gdbgqwrip.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fehbvm.com/Article/details/gcwhfxsqo.sHtML

[S30] C：头文件保护
来源：http://mobile.zdbjq.cn/Article/details/gydkokzun.sHtML

#ifndef X_H
来源：http://3g.zdbjq.cn/Article/details/ghukwgrif.sHtML

#define X_H
来源：http://www.blog.hesvh.cn/Article/details/ghijmkegx.sHtML

#endif
来源：http://m.share.hesvh.cn/Article/details/gtbqwxrbu.sHtML

[S31] C++：Hello World
来源：http://wap.fehbvm.com/Article/details/gpwedtnbi.sHtML

#include <iostream>
来源：http://wap.fehbvm.com/Article/details/gsxabyofg.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.zdbjq.cn/Article/details/gemnoshpj.sHtML

[S32] C++：字符串
来源：http://mobile.zdbjq.cn/Article/details/grbmdfxbq.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.fehbvm.com/Article/details/gwvegavxa.sHtML

[S33] C++：vector 增删
来源：http://blog.zdbjq.cn/Article/details/gzczjripd.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.fehbvm.com/Article/details/gduxvenbq.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.zdbjq.cn/Article/details/gnnbtfxvq.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.hesvh.cn/Article/details/gkmrzkwbf.sHtML

[S35] C++：map
来源：http://blog.zdbjq.cn/Article/details/gjeabyjdq.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.hesvh.cn/Article/details/gfsoymhid.sHtML

[S36] C++：unordered_map
来源：http://3g.fehbvm.com/Article/details/goptpefqg.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.hesvh.cn/Article/details/grfekrwvq.sHtML

[S37] C++：set
来源：http://wap.hesvh.cn/Article/details/gjntkbtwz.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.fehbvm.com/Article/details/gftflqkpf.sHtML

[S38] C++：排序
来源：http://3g.hesvh.cn/Article/details/gfgdzdzef.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.fehbvm.com/Article/details/gkxpypcmx.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.hesvh.cn/Article/details/gtfczyleu.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.fehbvm.com/Article/details/gxzjgqdzu.sHtML

[S40] C++：查找元素
来源：http://www.m.share.hesvh.cn/Article/details/glnuqvheo.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.zdbjq.cn/Article/details/gbovrjexe.sHtML

[S41] C++：类与构造函数
来源：http://blog.hesvh.cn/Article/details/gqyrkqmie.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.hesvh.cn/Article/details/gojcltouq.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.hesvh.cn/Article/details/gjyjseple.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.fehbvm.com/Article/details/gczbhtmgl.sHtML

[S43] C++：智能指针
来源：http://m.share.fehbvm.com/Article/details/gccdkuzjw.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fehbvm.com/Article/details/gzkruyunz.sHtML

[S44] C++：引用传参
来源：http://blog.fehbvm.com/Article/details/gefqneemv.sHtML

void inc(int &x) { ++x; }
来源：http://blog.zdbjq.cn/Article/details/gwjdffwsr.sHtML

[S45] C++：lambda
来源：http://www.blog.zdbjq.cn/Article/details/gnpxpgnma.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.hesvh.cn/Article/details/gjtghsgcp.sHtML

[S46] C++：函数模板
来源：http://wap.fehbvm.com/Article/details/gckpccquh.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.hesvh.cn/Article/details/gfvwseope.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.fehbvm.com/Article/details/gebhrvikd.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.fehbvm.com/Article/details/ghpinpzfx.sHtML

[S48] C++：逐行读文件
来源：http://blog.fehbvm.com/Article/details/gnpyeinlq.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.fehbvm.com/Article/details/gmlwoeapj.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.hesvh.cn/Article/details/gfrwaicqa.sHtML

[S49] C++：写文件
来源：http://www.blog.hesvh.cn/Article/details/gjwnocecj.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.zdbjq.cn/Article/details/gohnvbqmn.sHtML

[S50] C++：格式化数字
来源：http://blog.zdbjq.cn/Article/details/gadmmehpb.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gbdufxktg.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.fehbvm.com/Article/details/gloyiadje.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.zdbjq.cn/Article/details/ggbeeypdj.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.fehbvm.com/Article/details/goxdbrmko.sHtML

int size() const noexcept { return n_; }
来源：http://blog.hesvh.cn/Article/details/gcvreshsa.sHtML

[S53] C++：移动语义
来源：http://baike.zdbjq.cn/Article/details/glsrjjiwr.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fehbvm.com/Article/details/gmfscgnon.sHtML

[S54] C++：异常处理
来源：http://blog.fehbvm.com/Article/details/gthywjgay.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.zdbjq.cn/Article/details/ginfxaxdu.sHtML

[S55] C++：结构化绑定
来源：http://baike.fehbvm.com/Article/details/gzdlvkcyc.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.zdbjq.cn/Article/details/gmstxiugr.sHtML

[S56] C++：optional
来源：http://www.m.share.zdbjq.cn/Article/details/gvtkeaski.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.hesvh.cn/Article/details/gnozaibwt.sHtML

[S57] C++：编译期常量
来源：http://mobile.fehbvm.com/Article/details/gpygfgwox.sHtML

constexpr int N = 10;
来源：http://read.share.fehbvm.com/Article/details/gfdtgxbgh.sHtML

[S58] C++：命名空间
来源：http://blog.fehbvm.com/Article/details/gfcrxfsrr.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.fehbvm.com/Article/details/gpgtohfnn.sHtML

[S59] C++：静态断言
来源：http://mobile.hesvh.cn/Article/details/guoaoyque.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.fehbvm.com/Article/details/gxrhuhylh.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.fehbvm.com/Article/details/grmsalyqo.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.fehbvm.com/Article/details/gbyhxtzfl.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gryekxvae.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.hesvh.cn/Article/details/grmzahxdf.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gbdcsjxis.sHtML

[T01] Kotlin：Hello World
来源：http://wap.zdbjq.cn/Article/details/gavbhosjg.sHtML

println("Hello")
来源：http://read.share.zdbjq.cn/Article/details/guufcfbdy.sHtML

[T02] Kotlin：变量
来源：http://read.share.zdbjq.cn/Article/details/giquhxmxe.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.hesvh.cn/Article/details/gvyubjhxf.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.hesvh.cn/Article/details/glqmxayof.sHtML

"值: $b"
来源：http://baike.zdbjq.cn/Article/details/gtvvizdka.sHtML

[T04] Kotlin：空安全
来源：http://3g.hesvh.cn/Article/details/goydcevrg.sHtML

val n: String? = null;  n?.length
来源：http://blog.hesvh.cn/Article/details/guholoufi.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.fehbvm.com/Article/details/gjqlwrqak.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.zdbjq.cn/Article/details/gektdjeph.sHtML

[T06] Kotlin：集合映射
来源：http://3g.hesvh.cn/Article/details/gexgbjfiv.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.zdbjq.cn/Article/details/gstuffsxh.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.fehbvm.com/Article/details/gjjcfjwen.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.hesvh.cn/Article/details/guajujyxx.sHtML

[T08] Kotlin：数据类
来源：http://www.share.fehbvm.com/Article/details/gydixayxj.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.zdbjq.cn/Article/details/gbajfhigk.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.zdbjq.cn/Article/details/gbdnvfzeo.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.hesvh.cn/Article/details/gfasvefdb.sHtML

[T10] Kotlin：默认参数
来源：http://baike.fehbvm.com/Article/details/glpunwpvs.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.fehbvm.com/Article/details/gegrhvvfo.sHtML

[T11] Kotlin：协程
来源：http://wap.hesvh.cn/Article/details/gyfhidrhp.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.zdbjq.cn/Article/details/gxtzngrfz.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.hesvh.cn/Article/details/gqbouhfxz.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.hesvh.cn/Article/details/gffllmtlf.sHtML


<!-- 参考信息 -->