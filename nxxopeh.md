代发 wailian999

case "$1" in
来源：http://m.share.zdbjq.cn/Article/details/gxpgxvgfb.sHtML

start) echo "启动" ;;
来源：http://mobile.fehbvm.com/Article/details/gwoxteuvc.sHtML

stop)  echo "停止" ;;
来源：http://m.share.fehbvm.com/Article/details/gpjdarspm.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.fehbvm.com/Article/details/glwrhreeg.sHtML

esac
来源：http://blog.fehbvm.com/Article/details/gfmcijqak.sHtML

[R12] for 遍历文件
来源：http://baike.zdbjq.cn/Article/details/gsjxxxfzk.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.zdbjq.cn/Article/details/gnyhrsmke.sHtML

[R13] for 计数循环
来源：http://www.share.fehbvm.com/Article/details/gxdzijacy.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.hesvh.cn/Article/details/gzlsdcqxq.sHtML

[R14] C 风格 for
来源：http://www.m.share.hesvh.cn/Article/details/gwqzgcbnz.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.zdbjq.cn/Article/details/gdksaosmc.sHtML

[R15] while 逐行读文件
来源：http://3g.hesvh.cn/Article/details/gdprsxfla.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.zdbjq.cn/Article/details/gtwxfpvfw.sHtML

[R16] until 等待条件
来源：http://www.blog.fehbvm.com/Article/details/gmecznabr.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.hesvh.cn/Article/details/gyaixlbuy.sHtML

[R17] 数组定义与取值
来源：http://baike.zdbjq.cn/Article/details/guvhfcmxy.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.zdbjq.cn/Article/details/gcotgegal.sHtML

[R18] 遍历数组
来源：http://baike.zdbjq.cn/Article/details/gzjmkeixl.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.fehbvm.com/Article/details/gsozsnpee.sHtML

[R19] 数组长度
来源：http://mobile.hesvh.cn/Article/details/grxtcqmkj.sHtML

echo "${#arr[@]}"
来源：http://read.share.zdbjq.cn/Article/details/gbctuzvxm.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.zdbjq.cn/Article/details/gouutygzb.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.fehbvm.com/Article/details/gwkzjmqjq.sHtML

[R21] 字符串长度
来源：http://wap.hesvh.cn/Article/details/gmzoldzxr.sHtML

echo "${#s}"
来源：http://www.blog.zdbjq.cn/Article/details/gekivlwdc.sHtML

[R22] 截取子串
来源：http://3g.hesvh.cn/Article/details/glpppjtto.sHtML

echo "${s:0:5}"
来源：http://m.share.zdbjq.cn/Article/details/gncqyausz.sHtML

[R23] 字符串替换
来源：http://m.share.zdbjq.cn/Article/details/gnthcjrjg.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.zdbjq.cn/Article/details/gmlpffolr.sHtML

[R24] 大小写转换
来源：http://mobile.hesvh.cn/Article/details/gwwpojqjm.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.zdbjq.cn/Article/details/gopwupxoo.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.hesvh.cn/Article/details/gkursgvst.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.zdbjq.cn/Article/details/goodprvxt.sHtML

[R26] 命令替换
来源：http://www.m.share.fehbvm.com/Article/details/gnuzneyfk.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.hesvh.cn/Article/details/gmxalzgik.sHtML

[R27] 算术展开
来源：http://3g.fehbvm.com/Article/details/gujfwvxvq.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.hesvh.cn/Article/details/ggowfabfc.sHtML

[R28] 浮点运算
来源：http://blog.fehbvm.com/Article/details/gncfshfpm.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.zdbjq.cn/Article/details/gywbxdzwn.sHtML

[R29] 定义函数
来源：http://www.share.hesvh.cn/Article/details/grtogncra.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.hesvh.cn/Article/details/gkqzsokse.sHtML

[R30] 函数返回状态码
来源：http://www.blog.hesvh.cn/Article/details/gwnorfpam.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.zdbjq.cn/Article/details/gjigcbbcl.sHtML

[R31] 局部变量
来源：http://www.share.hesvh.cn/Article/details/gfpzvesbv.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.fehbvm.com/Article/details/gzheycrmv.sHtML

[R32] 参数个数校验
来源：http://read.share.fehbvm.com/Article/details/goecwmcyk.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.zdbjq.cn/Article/details/gkhquwzet.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.zdbjq.cn/Article/details/gkclycbbz.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.hesvh.cn/Article/details/gapuutocg.sHtML

[R34] 退出时清理
来源：http://www.m.share.hesvh.cn/Article/details/gbyfdaytg.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fehbvm.com/Article/details/gnnukzrqj.sHtML

[R35] 后台执行并等待
来源：http://www.blog.hesvh.cn/Article/details/gneofdiwi.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.fehbvm.com/Article/details/gohezprge.sHtML

[R36] 并发执行多个任务
来源：http://wap.hesvh.cn/Article/details/gyhyljapb.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.hesvh.cn/Article/details/gphphpvxc.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fehbvm.com/Article/details/gsshjrsjm.sHtML

files=$(ls -1)
来源：http://blog.hesvh.cn/Article/details/gufvohore.sHtML

[R38] 管道串联
来源：http://m.share.hesvh.cn/Article/details/gbhulgagp.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.hesvh.cn/Article/details/gberssmfx.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.hesvh.cn/Article/details/gjtgvjkkr.sHtML

cmd > out.log 2>&1
来源：http://www.blog.zdbjq.cn/Article/details/gablliwga.sHtML

[R40] 追加写日志
来源：http://www.m.share.zdbjq.cn/Article/details/gmaebawox.sHtML

echo "log" >> out.log
来源：http://3g.fehbvm.com/Article/details/gdsbgnnxr.sHtML

[R41] 丢弃输出
来源：http://mobile.fehbvm.com/Article/details/godvfgzyr.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.fehbvm.com/Article/details/gepissjsc.sHtML

[R42] 输入重定向
来源：http://baike.zdbjq.cn/Article/details/ggogzcugs.sHtML

wc -l < a.txt
来源：http://m.share.fehbvm.com/Article/details/glkppbtmk.sHtML

[R43] 按名字查找文件
来源：http://blog.zdbjq.cn/Article/details/gjisgzwcx.sHtML

find . -name "*.log" -type f
来源：http://www.share.hesvh.cn/Article/details/gfxflqoyv.sHtML

[R44] 按修改时间查找
来源：http://wap.zdbjq.cn/Article/details/gsulrsawh.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.fehbvm.com/Article/details/gfibdywjn.sHtML

[R45] 批量删除
来源：http://blog.hesvh.cn/Article/details/gsngmghxe.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fehbvm.com/Article/details/ggyhflugh.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fehbvm.com/Article/details/gvbjkyhtb.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.hesvh.cn/Article/details/gqqainylx.sHtML

[R47] sed 单行替换
来源：http://mobile.fehbvm.com/Article/details/gwiagyfkb.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.fehbvm.com/Article/details/gikxgypmz.sHtML

[R48] awk 取指定列
来源：http://www.m.share.zdbjq.cn/Article/details/gdmntixuz.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.hesvh.cn/Article/details/gxljwqius.sHtML

[R49] awk 带条件
来源：http://blog.zdbjq.cn/Article/details/ghhuexphf.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.zdbjq.cn/Article/details/gshndmhko.sHtML

[R50] awk 求和
来源：http://baike.fehbvm.com/Article/details/gchsvlpoj.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.fehbvm.com/Article/details/grnqhhmhm.sHtML

[R51] 排序去重取前几
来源：http://blog.zdbjq.cn/Article/details/gwuwsmxnn.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.hesvh.cn/Article/details/ggkoxycpu.sHtML

[R52] 统计行数
来源：http://www.blog.hesvh.cn/Article/details/gxhyhzvuz.sHtML

wc -l a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gvlutlcaq.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.hesvh.cn/Article/details/gbgskkxsz.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fehbvm.com/Article/details/gbpysanxj.sHtML

[R54] 比较两个文件
来源：http://read.share.fehbvm.com/Article/details/gzagmopqx.sHtML

diff a.txt b.txt
来源：http://read.share.hesvh.cn/Article/details/gotgfamhu.sHtML

[R55] 压缩与解压
来源：http://baike.zdbjq.cn/Article/details/glscsveqd.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fehbvm.com/Article/details/gerenlsot.sHtML

[R56] 远程拷贝
来源：http://blog.fehbvm.com/Article/details/gnsrbvnec.sHtML

scp file user@host:/path/
来源：http://mobile.zdbjq.cn/Article/details/gehxmdnwn.sHtML

[R57] 远程执行命令
来源：http://baike.zdbjq.cn/Article/details/gzgvtlxsj.sHtML

ssh user@host 'uptime'
来源：http://www.share.fehbvm.com/Article/details/gkjnrxdzw.sHtML

[R58] 下载文件
来源：http://www.blog.hesvh.cn/Article/details/gohoiteno.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.hesvh.cn/Article/details/gbwdskaoi.sHtML

[R59] 发 POST JSON
来源：http://blog.zdbjq.cn/Article/details/gkzrsvdtq.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.hesvh.cn/Article/details/gnocltlzu.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.zdbjq.cn/Article/details/gydiqfnlx.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.zdbjq.cn/Article/details/gvqlafzjo.sHtML

[R61] 磁盘占用
来源：http://www.blog.fehbvm.com/Article/details/ggpyeiwdh.sHtML

df -h;  du -sh *
来源：http://www.m.share.zdbjq.cn/Article/details/gyrwjfyyw.sHtML

[R62] 找最占空间的文件
来源：http://mobile.zdbjq.cn/Article/details/gffgegjhm.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.hesvh.cn/Article/details/gfqnnudvp.sHtML

[R63] 内存与进程
来源：http://www.share.fehbvm.com/Article/details/ggibfvmoi.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fehbvm.com/Article/details/gucyltnuz.sHtML

[R64] 结束进程
来源：http://3g.zdbjq.cn/Article/details/gmzpvmyih.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.hesvh.cn/Article/details/gkvlnbfgr.sHtML

[R65] 查看端口占用
来源：http://wap.zdbjq.cn/Article/details/guwczjrre.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.hesvh.cn/Article/details/gbotzvykr.sHtML

[R66] 定时任务
来源：http://wap.zdbjq.cn/Article/details/gjlaqvmpk.sHtML

crontab -e;  crontab -l
来源：http://blog.zdbjq.cn/Article/details/gdrtvdqim.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fehbvm.com/Article/details/gxggwhqxz.sHtML

openssl rand -hex 16
来源：http://mobile.hesvh.cn/Article/details/giqcohroh.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.zdbjq.cn/Article/details/gfhxgdctf.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fehbvm.com/Article/details/gdsaffxjq.sHtML

[R69] 生成随机密码
来源：http://wap.hesvh.cn/Article/details/gogaakluk.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.fehbvm.com/Article/details/gtzmuitdc.sHtML

[R70] 时间戳与互转
来源：http://mobile.hesvh.cn/Article/details/gtqlwuvaf.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fehbvm.com/Article/details/gazjrkiyx.sHtML

[R71] 日期格式化
来源：http://mobile.zdbjq.cn/Article/details/gpmccwpra.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.zdbjq.cn/Article/details/gqdtphcgj.sHtML

[R72] 等待端口就绪
来源：http://blog.fehbvm.com/Article/details/gqzemzrft.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.fehbvm.com/Article/details/gndadlrfw.sHtML

[R73] 分割大日志
来源：http://www.share.zdbjq.cn/Article/details/gehvkpwee.sHtML

split -l 1000 big.log part_
来源：http://mobile.zdbjq.cn/Article/details/gswhfvqgh.sHtML

[R74] 批量重命名
来源：http://3g.hesvh.cn/Article/details/gfxvfiisw.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.fehbvm.com/Article/details/gitxystub.sHtML

[R75] 导出环境变量
来源：http://m.share.fehbvm.com/Article/details/gmzfdkxzt.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.fehbvm.com/Article/details/gkzfoffpd.sHtML

[R76] 使用临时文件
来源：http://mobile.zdbjq.cn/Article/details/guxwqxmlh.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fehbvm.com/Article/details/gkeoacbxe.sHtML

[R77] 读取用户输入
来源：http://blog.hesvh.cn/Article/details/gwkgbaccv.sHtML

read -rp "请输入: " ans
来源：http://baike.hesvh.cn/Article/details/gfsyyyavg.sHtML

[R78] 交互式菜单
来源：http://baike.fehbvm.com/Article/details/geiclxjvc.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.zdbjq.cn/Article/details/gggfhuhhu.sHtML

[R79] 解析命令行选项
来源：http://read.share.hesvh.cn/Article/details/gtldkhoaq.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.hesvh.cn/Article/details/gobezjytu.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fehbvm.com/Article/details/gexcncqna.sHtML

time ./run.sh
来源：http://www.blog.zdbjq.cn/Article/details/gzbyqjhst.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gyiuudcfn.sHtML

S. C / C++ 专题
来源：http://www.share.zdbjq.cn/Article/details/gsqssbina.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gwjkdqzjf.sHtML

[S01] C：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gbtknhyjb.sHtML

#include <stdio.h>
来源：http://3g.hesvh.cn/Article/details/gsmtaijbk.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.zdbjq.cn/Article/details/gzrmxgahb.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.fehbvm.com/Article/details/glpnhuwbk.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fehbvm.com/Article/details/gkkjliska.sHtML

[S03] C：读入整数
来源：http://www.m.share.hesvh.cn/Article/details/ganqfagra.sHtML

int x; scanf("%d", &x);
来源：http://www.share.zdbjq.cn/Article/details/gtyiksrly.sHtML

[S04] C：字符串复制
来源：http://blog.fehbvm.com/Article/details/gvmewlgqh.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fehbvm.com/Article/details/gqwtugpho.sHtML

[S05] C：字符串长度
来源：http://read.share.hesvh.cn/Article/details/gcxkyhvpk.sHtML

strlen(s)
来源：http://mobile.zdbjq.cn/Article/details/gzzkicopb.sHtML

[S06] C：字符串比较
来源：http://wap.hesvh.cn/Article/details/givbcjchz.sHtML

strcmp(a, b) == 0
来源：http://www.blog.zdbjq.cn/Article/details/gpbvdzmdo.sHtML

[S07] C：数组遍历求和
来源：http://wap.zdbjq.cn/Article/details/ggsyjnztb.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.zdbjq.cn/Article/details/gnvbrdssl.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.zdbjq.cn/Article/details/gjsbriuoh.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.fehbvm.com/Article/details/goskhwurn.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fehbvm.com/Article/details/gadoudmmt.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.zdbjq.cn/Article/details/gzzrbxauh.sHtML

[S10] C：指针与解引用
来源：http://3g.hesvh.cn/Article/details/gmoeheuts.sHtML

int *p = &a;  *p = 5;
来源：http://baike.zdbjq.cn/Article/details/gxdiieaem.sHtML

[S11] C：逐行读文件
来源：http://3g.fehbvm.com/Article/details/gvydwsmjp.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.fehbvm.com/Article/details/gevbjcums.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.hesvh.cn/Article/details/ggxtzvfvt.sHtML

fclose(f);
来源：http://mobile.fehbvm.com/Article/details/gfthzfdyf.sHtML

[S12] C：写文件
来源：http://mobile.zdbjq.cn/Article/details/gbwkbnqur.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.zdbjq.cn/Article/details/guiumlyse.sHtML

[S13] C：宏定义
来源：http://www.share.hesvh.cn/Article/details/gehrblwax.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fehbvm.com/Article/details/gqcdvrmzk.sHtML

[S14] C：枚举
来源：http://3g.hesvh.cn/Article/details/ggrlnvzjc.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.zdbjq.cn/Article/details/gcsrbduof.sHtML

[S15] C：类型转换
来源：http://blog.hesvh.cn/Article/details/getpjhlur.sHtML

(double) a / b
来源：http://www.share.zdbjq.cn/Article/details/gufrciuik.sHtML

[S16] C：位操作置位
来源：http://read.share.zdbjq.cn/Article/details/gadzguwqv.sHtML

x |= (1 << 3);
来源：http://wap.fehbvm.com/Article/details/gbfjzhssk.sHtML

[S17] C：安全拼接字符串
来源：http://baike.hesvh.cn/Article/details/ghvmpefen.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.fehbvm.com/Article/details/gwjtblmlb.sHtML

[S18] C：命令行参数
来源：http://m.share.hesvh.cn/Article/details/geprutgxk.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.hesvh.cn/Article/details/gnjzaukhq.sHtML

[S19] C：快速排序
来源：http://www.share.zdbjq.cn/Article/details/grzyjyrod.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.fehbvm.com/Article/details/gciokthfe.sHtML

[S20] C：二分查找
来源：http://www.blog.fehbvm.com/Article/details/gbjzozyge.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.hesvh.cn/Article/details/glqurtzvq.sHtML

[S21] C：字符类别判断
来源：http://baike.fehbvm.com/Article/details/gxhnylkhj.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.hesvh.cn/Article/details/gxbrwtlou.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fehbvm.com/Article/details/gyzfsspoj.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.hesvh.cn/Article/details/gtscoluai.sHtML

[S23] C：随机数
来源：http://blog.fehbvm.com/Article/details/grgsgmlzv.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.fehbvm.com/Article/details/ggpkhawmh.sHtML

[S24] C：获取本地时间
来源：http://read.share.zdbjq.cn/Article/details/grktovjan.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.zdbjq.cn/Article/details/gewwtskxb.sHtML

[S25] C：内存拷贝
来源：http://read.share.hesvh.cn/Article/details/geazdvtgy.sHtML

memcpy(dst, src, n);
来源：http://wap.hesvh.cn/Article/details/gswcghlmy.sHtML

[S26] C：内存清零
来源：http://www.blog.hesvh.cn/Article/details/gtdkgkxoh.sHtML

memset(a, 0, sizeof a);
来源：http://blog.hesvh.cn/Article/details/gjiqlkifc.sHtML

[S27] C：定义常量
来源：http://mobile.hesvh.cn/Article/details/gibnanuvo.sHtML

const double PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gttqhrtyz.sHtML

[S28] C：静态变量
来源：http://www.m.share.zdbjq.cn/Article/details/ghstmybub.sHtML

static int counter = 0;
来源：http://baike.zdbjq.cn/Article/details/gynnouvmg.sHtML

[S29] C：变参函数
来源：http://baike.zdbjq.cn/Article/details/gauwbfjgv.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fehbvm.com/Article/details/gxuctxtoi.sHtML

[S30] C：头文件保护
来源：http://read.share.fehbvm.com/Article/details/gahoqknou.sHtML

#ifndef X_H
来源：http://m.share.zdbjq.cn/Article/details/gdrbyjxga.sHtML

#define X_H
来源：http://www.blog.zdbjq.cn/Article/details/gdsjpjehi.sHtML

#endif
来源：http://read.share.fehbvm.com/Article/details/ggmqritys.sHtML

[S31] C++：Hello World
来源：http://baike.fehbvm.com/Article/details/gtqvvpbhv.sHtML

#include <iostream>
来源：http://www.blog.zdbjq.cn/Article/details/gtckersvq.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.fehbvm.com/Article/details/gnddsbjjf.sHtML

[S32] C++：字符串
来源：http://blog.fehbvm.com/Article/details/gjxyhiqje.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.hesvh.cn/Article/details/gljpnwthl.sHtML

[S33] C++：vector 增删
来源：http://3g.zdbjq.cn/Article/details/gkckhymfb.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.fehbvm.com/Article/details/gmqyymzkj.sHtML

[S34] C++：遍历 vector
来源：http://read.share.hesvh.cn/Article/details/ggnimjcri.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.hesvh.cn/Article/details/gntiklmbl.sHtML

[S35] C++：map
来源：http://baike.zdbjq.cn/Article/details/gqiilqwra.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fehbvm.com/Article/details/gopdlwuqz.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.fehbvm.com/Article/details/gmskyjiie.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gpnstmyhq.sHtML

[S37] C++：set
来源：http://wap.hesvh.cn/Article/details/gwdahbitw.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.fehbvm.com/Article/details/gffrdhvqa.sHtML

[S38] C++：排序
来源：http://blog.hesvh.cn/Article/details/gwemetrii.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.hesvh.cn/Article/details/gjhbwhyip.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.hesvh.cn/Article/details/gnoxrtxhw.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.hesvh.cn/Article/details/gtwmpgkka.sHtML

[S40] C++：查找元素
来源：http://blog.fehbvm.com/Article/details/gozrbizlv.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.fehbvm.com/Article/details/gvufrcook.sHtML

[S41] C++：类与构造函数
来源：http://baike.fehbvm.com/Article/details/gwehoxufw.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.hesvh.cn/Article/details/gdknktutp.sHtML

[S42] C++：继承与虚函数
来源：http://3g.hesvh.cn/Article/details/ghmsmonlq.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.zdbjq.cn/Article/details/gdbljxdxv.sHtML

[S43] C++：智能指针
来源：http://blog.fehbvm.com/Article/details/gexwywdbi.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.hesvh.cn/Article/details/grrghjysx.sHtML

[S44] C++：引用传参
来源：http://3g.hesvh.cn/Article/details/gqnxzqqjh.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.zdbjq.cn/Article/details/gzueaovye.sHtML

[S45] C++：lambda
来源：http://wap.zdbjq.cn/Article/details/gxrfdbdrf.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.fehbvm.com/Article/details/gksygfmxy.sHtML

[S46] C++：函数模板
来源：http://blog.hesvh.cn/Article/details/gvvtirgkt.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.zdbjq.cn/Article/details/gyymwlctp.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.fehbvm.com/Article/details/ghruiouaq.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.hesvh.cn/Article/details/gvbpsdugs.sHtML

[S48] C++：逐行读文件
来源：http://wap.hesvh.cn/Article/details/gezlnrbsj.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.zdbjq.cn/Article/details/gxexwxsto.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.hesvh.cn/Article/details/gpacgedtf.sHtML

[S49] C++：写文件
来源：http://3g.fehbvm.com/Article/details/gbaxfylpu.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.zdbjq.cn/Article/details/gfiekypdp.sHtML

[S50] C++：格式化数字
来源：http://mobile.hesvh.cn/Article/details/ggusadzes.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gcgmwssvl.sHtML

[S51] C++：显式类型转换
来源：http://3g.hesvh.cn/Article/details/gmpzehwmr.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.fehbvm.com/Article/details/gbmptplrv.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.zdbjq.cn/Article/details/gysjuyjkd.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.zdbjq.cn/Article/details/gphalzsyl.sHtML

[S53] C++：移动语义
来源：http://www.blog.zdbjq.cn/Article/details/glshciaoz.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.hesvh.cn/Article/details/gknsiejcz.sHtML

[S54] C++：异常处理
来源：http://www.blog.fehbvm.com/Article/details/gjwppnzjr.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.zdbjq.cn/Article/details/ggzmfyaen.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.fehbvm.com/Article/details/guuullgcz.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.zdbjq.cn/Article/details/gzgdzuine.sHtML

[S56] C++：optional
来源：http://m.share.hesvh.cn/Article/details/grttlftcf.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.fehbvm.com/Article/details/gnvwmngqu.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.hesvh.cn/Article/details/gqswxiazt.sHtML

constexpr int N = 10;
来源：http://3g.hesvh.cn/Article/details/gxezlekrg.sHtML

[S58] C++：命名空间
来源：http://blog.fehbvm.com/Article/details/gzlgxddpr.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.fehbvm.com/Article/details/gabzstoxq.sHtML

[S59] C++：静态断言
来源：http://m.share.zdbjq.cn/Article/details/gnhilthtq.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.hesvh.cn/Article/details/ghynkwgzm.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.fehbvm.com/Article/details/gdsookcal.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.zdbjq.cn/Article/details/gffgwlghf.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gcvlcsawm.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.hesvh.cn/Article/details/gzdkovqbm.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gskdttqhh.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.zdbjq.cn/Article/details/giazkizuh.sHtML

println("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gbdagrewv.sHtML

[T02] Kotlin：变量
来源：http://3g.fehbvm.com/Article/details/gykwemwhu.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.fehbvm.com/Article/details/gbsjtnqvg.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.hesvh.cn/Article/details/grptvuysj.sHtML

"值: $b"
来源：http://3g.fehbvm.com/Article/details/gkpzmagxq.sHtML

[T04] Kotlin：空安全
来源：http://mobile.zdbjq.cn/Article/details/gjmawahjc.sHtML

val n: String? = null;  n?.length
来源：http://mobile.zdbjq.cn/Article/details/gswhnptxo.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.fehbvm.com/Article/details/grilolnjq.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.hesvh.cn/Article/details/gpgvfoxbx.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.fehbvm.com/Article/details/gdgelalse.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.hesvh.cn/Article/details/gqpzigqlb.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.hesvh.cn/Article/details/gaposzopg.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.zdbjq.cn/Article/details/gqgtdqdos.sHtML

[T08] Kotlin：数据类
来源：http://wap.fehbvm.com/Article/details/gzxabowjd.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.zdbjq.cn/Article/details/gqoobktll.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.fehbvm.com/Article/details/gvuuawror.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.zdbjq.cn/Article/details/gtmdwpmav.sHtML

[T10] Kotlin：默认参数
来源：http://3g.fehbvm.com/Article/details/gbbggkhgp.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.fehbvm.com/Article/details/gunebieqg.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.hesvh.cn/Article/details/gqvkgbino.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.zdbjq.cn/Article/details/gtciszqza.sHtML

[T12] Kotlin：解构声明
来源：http://wap.zdbjq.cn/Article/details/ghlmsmhvo.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.hesvh.cn/Article/details/gctgahqzm.sHtML


<!-- 参考信息 -->