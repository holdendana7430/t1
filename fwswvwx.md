代发 wailian999

case "$1" in
来源：http://www.m.share.fehbvm.com/Article/details/gczbcizpy.sHtML

start) echo "启动" ;;
来源：http://read.share.hesvh.cn/Article/details/glbpatgpa.sHtML

stop)  echo "停止" ;;
来源：http://baike.fehbvm.com/Article/details/ghbwacltn.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.hesvh.cn/Article/details/gmaydugzh.sHtML

esac
来源：http://www.blog.fehbvm.com/Article/details/gzxaggsyj.sHtML

[R12] for 遍历文件
来源：http://m.share.fehbvm.com/Article/details/goqublxbo.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.hesvh.cn/Article/details/gwqabjqyd.sHtML

[R13] for 计数循环
来源：http://www.share.fehbvm.com/Article/details/gxywmahqe.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.hesvh.cn/Article/details/gqhuvmzjo.sHtML

[R14] C 风格 for
来源：http://baike.fehbvm.com/Article/details/gvtyopwfd.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.fehbvm.com/Article/details/gbcpngoen.sHtML

[R15] while 逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gqfevelyf.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.zdbjq.cn/Article/details/gloaylyov.sHtML

[R16] until 等待条件
来源：http://baike.hesvh.cn/Article/details/gijhemkra.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.fehbvm.com/Article/details/gfpcnyzlc.sHtML

[R17] 数组定义与取值
来源：http://baike.fehbvm.com/Article/details/gqoschkde.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.zdbjq.cn/Article/details/grqcwgdjg.sHtML

[R18] 遍历数组
来源：http://wap.hesvh.cn/Article/details/golayyqfb.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.fehbvm.com/Article/details/gfqaucsxs.sHtML

[R19] 数组长度
来源：http://www.share.hesvh.cn/Article/details/gyhxcybvb.sHtML

echo "${#arr[@]}"
来源：http://3g.hesvh.cn/Article/details/gbywhaiuv.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.hesvh.cn/Article/details/grrqcqgta.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.hesvh.cn/Article/details/gggcdizuk.sHtML

[R21] 字符串长度
来源：http://read.share.fehbvm.com/Article/details/gppwjeoif.sHtML

echo "${#s}"
来源：http://wap.zdbjq.cn/Article/details/gaypulvkg.sHtML

[R22] 截取子串
来源：http://baike.fehbvm.com/Article/details/glkwokikk.sHtML

echo "${s:0:5}"
来源：http://mobile.fehbvm.com/Article/details/grahdgtca.sHtML

[R23] 字符串替换
来源：http://mobile.hesvh.cn/Article/details/gzozxpmcb.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.zdbjq.cn/Article/details/gzyvyscmh.sHtML

[R24] 大小写转换
来源：http://baike.zdbjq.cn/Article/details/gvbvwrnim.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.fehbvm.com/Article/details/gjhnrsloi.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.zdbjq.cn/Article/details/gzczfrclx.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.hesvh.cn/Article/details/gaufgjlmm.sHtML

[R26] 命令替换
来源：http://www.m.share.fehbvm.com/Article/details/gcajptqyx.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.zdbjq.cn/Article/details/glfrgntuv.sHtML

[R27] 算术展开
来源：http://m.share.fehbvm.com/Article/details/gzyozfwdt.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.hesvh.cn/Article/details/gidjskxko.sHtML

[R28] 浮点运算
来源：http://3g.zdbjq.cn/Article/details/gbusljeym.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.hesvh.cn/Article/details/guwvkuzet.sHtML

[R29] 定义函数
来源：http://m.share.fehbvm.com/Article/details/gjzwcnwaf.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.hesvh.cn/Article/details/gtdmwtszy.sHtML

[R30] 函数返回状态码
来源：http://blog.zdbjq.cn/Article/details/gacnmzthb.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.zdbjq.cn/Article/details/gscqmxxyc.sHtML

[R31] 局部变量
来源：http://blog.zdbjq.cn/Article/details/gsxqsebgy.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gnscdkxtf.sHtML

[R32] 参数个数校验
来源：http://www.m.share.hesvh.cn/Article/details/ghbtpcohw.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.zdbjq.cn/Article/details/grxqrvjbq.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.hesvh.cn/Article/details/gbkdrxkbk.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.hesvh.cn/Article/details/giobvbgnm.sHtML

[R34] 退出时清理
来源：http://read.share.fehbvm.com/Article/details/gicghqrom.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.zdbjq.cn/Article/details/gnpkqyoph.sHtML

[R35] 后台执行并等待
来源：http://wap.zdbjq.cn/Article/details/gqcoqnwmt.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.hesvh.cn/Article/details/gosnnfelt.sHtML

[R36] 并发执行多个任务
来源：http://read.share.zdbjq.cn/Article/details/gsbvnqhdd.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.hesvh.cn/Article/details/gaiykyonv.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.zdbjq.cn/Article/details/gqsvzqvqe.sHtML

files=$(ls -1)
来源：http://www.blog.hesvh.cn/Article/details/gdacihgcq.sHtML

[R38] 管道串联
来源：http://wap.fehbvm.com/Article/details/gwqslxkfw.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.hesvh.cn/Article/details/gvtwtxtwa.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.zdbjq.cn/Article/details/guwnzqxqt.sHtML

cmd > out.log 2>&1
来源：http://mobile.fehbvm.com/Article/details/gvzdmozam.sHtML

[R40] 追加写日志
来源：http://read.share.zdbjq.cn/Article/details/gtvvmlzml.sHtML

echo "log" >> out.log
来源：http://www.blog.fehbvm.com/Article/details/gfraglbsm.sHtML

[R41] 丢弃输出
来源：http://www.share.zdbjq.cn/Article/details/gcpkxbqek.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.zdbjq.cn/Article/details/gllvvkgcr.sHtML

[R42] 输入重定向
来源：http://www.m.share.fehbvm.com/Article/details/gffhlevtq.sHtML

wc -l < a.txt
来源：http://mobile.zdbjq.cn/Article/details/gwvcecpap.sHtML

[R43] 按名字查找文件
来源：http://read.share.hesvh.cn/Article/details/gthqrfvec.sHtML

find . -name "*.log" -type f
来源：http://www.blog.zdbjq.cn/Article/details/grdyuacbx.sHtML

[R44] 按修改时间查找
来源：http://wap.fehbvm.com/Article/details/grvcezoco.sHtML

find . -mtime -7 -type f
来源：http://mobile.fehbvm.com/Article/details/gobmluagy.sHtML

[R45] 批量删除
来源：http://3g.zdbjq.cn/Article/details/gjzjjyddl.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.hesvh.cn/Article/details/guzbythmt.sHtML

[R46] 递归替换文件内容
来源：http://baike.zdbjq.cn/Article/details/gimwccsoe.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fehbvm.com/Article/details/ghelzcryv.sHtML

[R47] sed 单行替换
来源：http://www.share.hesvh.cn/Article/details/gsjmztaoq.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fehbvm.com/Article/details/gnosqhbbc.sHtML

[R48] awk 取指定列
来源：http://read.share.hesvh.cn/Article/details/gwotppjwa.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.zdbjq.cn/Article/details/ginlrretu.sHtML

[R49] awk 带条件
来源：http://blog.zdbjq.cn/Article/details/gvbxhuzev.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fehbvm.com/Article/details/gsukjggkh.sHtML

[R50] awk 求和
来源：http://www.share.fehbvm.com/Article/details/gqpzgysar.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.zdbjq.cn/Article/details/gpeqihqay.sHtML

[R51] 排序去重取前几
来源：http://blog.fehbvm.com/Article/details/gxolbtbyz.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.hesvh.cn/Article/details/gmfdnngwu.sHtML

[R52] 统计行数
来源：http://read.share.fehbvm.com/Article/details/ggogorkcz.sHtML

wc -l a.txt
来源：http://www.blog.fehbvm.com/Article/details/gfnzvlyql.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fehbvm.com/Article/details/gfbbmepdg.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.hesvh.cn/Article/details/gcptdjpce.sHtML

[R54] 比较两个文件
来源：http://www.share.zdbjq.cn/Article/details/gilmbkuji.sHtML

diff a.txt b.txt
来源：http://baike.fehbvm.com/Article/details/grerhdsso.sHtML

[R55] 压缩与解压
来源：http://www.blog.hesvh.cn/Article/details/gtmfmwesk.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.zdbjq.cn/Article/details/gqotyjprf.sHtML

[R56] 远程拷贝
来源：http://www.share.fehbvm.com/Article/details/gciagfwne.sHtML

scp file user@host:/path/
来源：http://mobile.zdbjq.cn/Article/details/geifcfuas.sHtML

[R57] 远程执行命令
来源：http://mobile.zdbjq.cn/Article/details/gpyuximri.sHtML

ssh user@host 'uptime'
来源：http://m.share.fehbvm.com/Article/details/gtvnnwjdj.sHtML

[R58] 下载文件
来源：http://read.share.fehbvm.com/Article/details/ghveeibbw.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fehbvm.com/Article/details/ghkzbadxz.sHtML

[R59] 发 POST JSON
来源：http://3g.hesvh.cn/Article/details/gerrnqwud.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.zdbjq.cn/Article/details/gkpsuzpdg.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.zdbjq.cn/Article/details/gjzgesmwm.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.zdbjq.cn/Article/details/gsybvxaei.sHtML

[R61] 磁盘占用
来源：http://mobile.zdbjq.cn/Article/details/gpppmbcni.sHtML

df -h;  du -sh *
来源：http://mobile.zdbjq.cn/Article/details/gizorgohg.sHtML

[R62] 找最占空间的文件
来源：http://mobile.hesvh.cn/Article/details/gbafzidoe.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.zdbjq.cn/Article/details/gmiaaejtd.sHtML

[R63] 内存与进程
来源：http://blog.zdbjq.cn/Article/details/ggrluzoyn.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.zdbjq.cn/Article/details/gjdfryvgj.sHtML

[R64] 结束进程
来源：http://www.blog.fehbvm.com/Article/details/gfhojtiwc.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.zdbjq.cn/Article/details/gfkvkqqqt.sHtML

[R65] 查看端口占用
来源：http://3g.fehbvm.com/Article/details/gybyymbkh.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.hesvh.cn/Article/details/gvtuotesj.sHtML

[R66] 定时任务
来源：http://3g.hesvh.cn/Article/details/gxtuvfkxm.sHtML

crontab -e;  crontab -l
来源：http://www.blog.hesvh.cn/Article/details/gramwvqmi.sHtML

[R67] 生成随机十六进制串
来源：http://baike.hesvh.cn/Article/details/gkkqrtetb.sHtML

openssl rand -hex 16
来源：http://www.blog.fehbvm.com/Article/details/gcrhvtsbz.sHtML

[R68] 计算文件校验值
来源：http://read.share.hesvh.cn/Article/details/gjujylxnj.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fehbvm.com/Article/details/gcdecsmbl.sHtML

[R69] 生成随机密码
来源：http://blog.hesvh.cn/Article/details/gtnybxfty.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.zdbjq.cn/Article/details/gfajlivcn.sHtML

[R70] 时间戳与互转
来源：http://baike.fehbvm.com/Article/details/gbsioovra.sHtML

date +%s;  date -d @1700000000
来源：http://blog.zdbjq.cn/Article/details/gavvnukin.sHtML

[R71] 日期格式化
来源：http://www.share.fehbvm.com/Article/details/gyszozysp.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.hesvh.cn/Article/details/ggelkbuan.sHtML

[R72] 等待端口就绪
来源：http://wap.zdbjq.cn/Article/details/gkayqckfk.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.hesvh.cn/Article/details/gfftwinrj.sHtML

[R73] 分割大日志
来源：http://www.blog.hesvh.cn/Article/details/gcbuwqsjh.sHtML

split -l 1000 big.log part_
来源：http://blog.fehbvm.com/Article/details/giokmoqgu.sHtML

[R74] 批量重命名
来源：http://www.share.zdbjq.cn/Article/details/gqcrmjtue.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.hesvh.cn/Article/details/gwrpbvriu.sHtML

[R75] 导出环境变量
来源：http://m.share.zdbjq.cn/Article/details/gnkrwotwc.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.hesvh.cn/Article/details/gigppuwjv.sHtML

[R76] 使用临时文件
来源：http://www.blog.fehbvm.com/Article/details/ggbcuqvgy.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.hesvh.cn/Article/details/gzqaatrgf.sHtML

[R77] 读取用户输入
来源：http://read.share.fehbvm.com/Article/details/gsnxnokbd.sHtML

read -rp "请输入: " ans
来源：http://3g.fehbvm.com/Article/details/gveloashy.sHtML

[R78] 交互式菜单
来源：http://read.share.fehbvm.com/Article/details/greenlsnr.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fehbvm.com/Article/details/glihzdlur.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.zdbjq.cn/Article/details/gaekzvqvy.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.hesvh.cn/Article/details/gdxkcbqme.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.zdbjq.cn/Article/details/gqpgebqrk.sHtML

time ./run.sh
来源：http://www.share.zdbjq.cn/Article/details/gpfiikjly.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gkyjhcpjo.sHtML

S. C / C++ 专题
来源：http://blog.fehbvm.com/Article/details/gkgsqyoyv.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gkhopfwik.sHtML

[S01] C：Hello World
来源：http://m.share.fehbvm.com/Article/details/gdrejazje.sHtML

#include <stdio.h>
来源：http://www.blog.hesvh.cn/Article/details/gaelwokko.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fehbvm.com/Article/details/ggrqwlrsr.sHtML

[S02] C：变量与格式化输出
来源：http://blog.fehbvm.com/Article/details/ghgaswvkh.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.hesvh.cn/Article/details/gqzphewtj.sHtML

[S03] C：读入整数
来源：http://read.share.zdbjq.cn/Article/details/gqnjheqfd.sHtML

int x; scanf("%d", &x);
来源：http://3g.zdbjq.cn/Article/details/gggdfpxgl.sHtML

[S04] C：字符串复制
来源：http://read.share.fehbvm.com/Article/details/gfzvtrtem.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.hesvh.cn/Article/details/ggsoikcui.sHtML

[S05] C：字符串长度
来源：http://www.share.hesvh.cn/Article/details/gumzdkwjv.sHtML

strlen(s)
来源：http://blog.hesvh.cn/Article/details/gdxravpxo.sHtML

[S06] C：字符串比较
来源：http://baike.fehbvm.com/Article/details/gxmrdttrt.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.hesvh.cn/Article/details/gdjesodck.sHtML

[S07] C：数组遍历求和
来源：http://www.share.fehbvm.com/Article/details/gecxshvbt.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.hesvh.cn/Article/details/gbnkkxibz.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.hesvh.cn/Article/details/gtjvsgnaa.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.hesvh.cn/Article/details/gkcqiqlpv.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fehbvm.com/Article/details/guqvneenq.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.hesvh.cn/Article/details/guivttmzc.sHtML

[S10] C：指针与解引用
来源：http://www.blog.zdbjq.cn/Article/details/gppcnauvu.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.hesvh.cn/Article/details/gcfmgvvmz.sHtML

[S11] C：逐行读文件
来源：http://3g.hesvh.cn/Article/details/gaucewfdy.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.hesvh.cn/Article/details/gsarjoobo.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.hesvh.cn/Article/details/gudwdeygr.sHtML

fclose(f);
来源：http://3g.fehbvm.com/Article/details/gronmfxya.sHtML

[S12] C：写文件
来源：http://mobile.hesvh.cn/Article/details/gipsezyul.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.zdbjq.cn/Article/details/glyzjusql.sHtML

[S13] C：宏定义
来源：http://www.m.share.fehbvm.com/Article/details/gawmavhen.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.hesvh.cn/Article/details/gnomdzomr.sHtML

[S14] C：枚举
来源：http://3g.zdbjq.cn/Article/details/giyfgdejd.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.zdbjq.cn/Article/details/gemkxregy.sHtML

[S15] C：类型转换
来源：http://m.share.zdbjq.cn/Article/details/gkoldaqbz.sHtML

(double) a / b
来源：http://mobile.fehbvm.com/Article/details/gleuamasx.sHtML

[S16] C：位操作置位
来源：http://wap.fehbvm.com/Article/details/gpngbxouh.sHtML

x |= (1 << 3);
来源：http://www.m.share.fehbvm.com/Article/details/gknozzfeq.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gwijmhnwg.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.hesvh.cn/Article/details/gnicmkayw.sHtML

[S18] C：命令行参数
来源：http://www.blog.hesvh.cn/Article/details/gdqrudkbv.sHtML

int main(int argc, char **argv)
来源：http://read.share.zdbjq.cn/Article/details/gjfxzcxlc.sHtML

[S19] C：快速排序
来源：http://m.share.zdbjq.cn/Article/details/gshmbhnrz.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fehbvm.com/Article/details/grgthssin.sHtML

[S20] C：二分查找
来源：http://mobile.hesvh.cn/Article/details/grraabrdt.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.hesvh.cn/Article/details/gxqjpkqrx.sHtML

[S21] C：字符类别判断
来源：http://blog.fehbvm.com/Article/details/gfxcfdbvq.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fehbvm.com/Article/details/gpuojxpzj.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.hesvh.cn/Article/details/genqcudle.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.hesvh.cn/Article/details/gmnsiltas.sHtML

[S23] C：随机数
来源：http://mobile.zdbjq.cn/Article/details/gmwrnowwc.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.hesvh.cn/Article/details/glmszecny.sHtML

[S24] C：获取本地时间
来源：http://www.blog.zdbjq.cn/Article/details/gkzahhxst.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.hesvh.cn/Article/details/gmzufxhuk.sHtML

[S25] C：内存拷贝
来源：http://read.share.hesvh.cn/Article/details/goddbtwqw.sHtML

memcpy(dst, src, n);
来源：http://baike.fehbvm.com/Article/details/gkcahqmtj.sHtML

[S26] C：内存清零
来源：http://read.share.hesvh.cn/Article/details/gupyfoyga.sHtML

memset(a, 0, sizeof a);
来源：http://blog.zdbjq.cn/Article/details/gqboxxstz.sHtML

[S27] C：定义常量
来源：http://wap.hesvh.cn/Article/details/gbdkgadxg.sHtML

const double PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/ggutwprlk.sHtML

[S28] C：静态变量
来源：http://www.blog.hesvh.cn/Article/details/gshplbkrp.sHtML

static int counter = 0;
来源：http://mobile.zdbjq.cn/Article/details/gxynkxoff.sHtML

[S29] C：变参函数
来源：http://wap.fehbvm.com/Article/details/gucrlsoqp.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.zdbjq.cn/Article/details/ggewvwbab.sHtML

[S30] C：头文件保护
来源：http://blog.zdbjq.cn/Article/details/grwjmdmkv.sHtML

#ifndef X_H
来源：http://wap.fehbvm.com/Article/details/gacasvxfj.sHtML

#define X_H
来源：http://baike.zdbjq.cn/Article/details/gqamfmzkd.sHtML

#endif
来源：http://blog.fehbvm.com/Article/details/gshxwxsvt.sHtML

[S31] C++：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gqmibajmd.sHtML

#include <iostream>
来源：http://blog.fehbvm.com/Article/details/gyhxvywvs.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.hesvh.cn/Article/details/gilnbatgs.sHtML

[S32] C++：字符串
来源：http://www.blog.zdbjq.cn/Article/details/gbwsabjdj.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fehbvm.com/Article/details/gqdgebgoj.sHtML

[S33] C++：vector 增删
来源：http://3g.fehbvm.com/Article/details/ghhjbxhjk.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.hesvh.cn/Article/details/gnhcxrzgj.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.fehbvm.com/Article/details/goochhlqz.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fehbvm.com/Article/details/gnucawewr.sHtML

[S35] C++：map
来源：http://read.share.zdbjq.cn/Article/details/gbutkcath.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/gzcjnurpx.sHtML

[S36] C++：unordered_map
来源：http://m.share.fehbvm.com/Article/details/gpilpnlum.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/grsvdsbad.sHtML

[S37] C++：set
来源：http://www.share.fehbvm.com/Article/details/gfovntkan.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fehbvm.com/Article/details/gvkdcanho.sHtML

[S38] C++：排序
来源：http://wap.hesvh.cn/Article/details/ghhxmzkms.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.zdbjq.cn/Article/details/gcadounja.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.zdbjq.cn/Article/details/gmqqnnqvy.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.zdbjq.cn/Article/details/gterwcypz.sHtML

[S40] C++：查找元素
来源：http://www.m.share.fehbvm.com/Article/details/gscunuaag.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.fehbvm.com/Article/details/gtjhnenjj.sHtML

[S41] C++：类与构造函数
来源：http://www.share.hesvh.cn/Article/details/gyvofrdgy.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.fehbvm.com/Article/details/gnepvygwp.sHtML

[S42] C++：继承与虚函数
来源：http://3g.hesvh.cn/Article/details/gtabhsfgd.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.zdbjq.cn/Article/details/gcrahnjqw.sHtML

[S43] C++：智能指针
来源：http://www.blog.zdbjq.cn/Article/details/gqmxqvrya.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.fehbvm.com/Article/details/gmnqxtsme.sHtML

[S44] C++：引用传参
来源：http://3g.hesvh.cn/Article/details/gkkxkscfr.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.fehbvm.com/Article/details/gdmmuoofe.sHtML

[S45] C++：lambda
来源：http://www.m.share.fehbvm.com/Article/details/gaavnmadk.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.zdbjq.cn/Article/details/gwaimvpym.sHtML

[S46] C++：函数模板
来源：http://www.m.share.fehbvm.com/Article/details/gzmdcjrcy.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.fehbvm.com/Article/details/gbxzyldxg.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.hesvh.cn/Article/details/gemgobxzk.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.hesvh.cn/Article/details/gefgorave.sHtML

[S48] C++：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gqlvhhrdw.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.zdbjq.cn/Article/details/gxsxfpfwn.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.hesvh.cn/Article/details/grnsthbwr.sHtML

[S49] C++：写文件
来源：http://read.share.fehbvm.com/Article/details/gdcfytfma.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.hesvh.cn/Article/details/gubgbjipd.sHtML

[S50] C++：格式化数字
来源：http://www.blog.fehbvm.com/Article/details/gxokmzlxd.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gozksiiau.sHtML

[S51] C++：显式类型转换
来源：http://baike.zdbjq.cn/Article/details/gensswgud.sHtML

static_cast<double>(a) / b
来源：http://m.share.fehbvm.com/Article/details/grsmxxayc.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.zdbjq.cn/Article/details/gavbxnvsr.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.fehbvm.com/Article/details/ghxozwiwy.sHtML

[S53] C++：移动语义
来源：http://3g.zdbjq.cn/Article/details/gfybpugsh.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.fehbvm.com/Article/details/gtwzqssga.sHtML

[S54] C++：异常处理
来源：http://www.blog.hesvh.cn/Article/details/gkszdioir.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.zdbjq.cn/Article/details/gvezxlkzd.sHtML

[S55] C++：结构化绑定
来源：http://blog.hesvh.cn/Article/details/gluuylqfi.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.fehbvm.com/Article/details/ggxmwfvjn.sHtML

[S56] C++：optional
来源：http://www.m.share.fehbvm.com/Article/details/gpppvziaz.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.fehbvm.com/Article/details/gcptutrme.sHtML

[S57] C++：编译期常量
来源：http://www.share.fehbvm.com/Article/details/gunasipoi.sHtML

constexpr int N = 10;
来源：http://wap.zdbjq.cn/Article/details/gmodjzkaq.sHtML

[S58] C++：命名空间
来源：http://m.share.fehbvm.com/Article/details/gtxeeenxt.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.zdbjq.cn/Article/details/gjzzkbnxe.sHtML

[S59] C++：静态断言
来源：http://www.share.fehbvm.com/Article/details/gqdxrqvbv.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fehbvm.com/Article/details/gnxngdjfe.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.hesvh.cn/Article/details/grrtzztaw.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.hesvh.cn/Article/details/gogkympcj.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gdeirfptp.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fehbvm.com/Article/details/gncwnbgha.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gzwozamtj.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gjrvphddu.sHtML

println("Hello")
来源：http://blog.hesvh.cn/Article/details/grvrkdkoa.sHtML

[T02] Kotlin：变量
来源：http://baike.fehbvm.com/Article/details/grggfndll.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.fehbvm.com/Article/details/gcyyuexuj.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.hesvh.cn/Article/details/gddcbesfv.sHtML

"值: $b"
来源：http://wap.zdbjq.cn/Article/details/gcuefyvaq.sHtML

[T04] Kotlin：空安全
来源：http://read.share.hesvh.cn/Article/details/gotzfnvmu.sHtML

val n: String? = null;  n?.length
来源：http://3g.fehbvm.com/Article/details/gdtjjxodg.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.zdbjq.cn/Article/details/gkozawkin.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.fehbvm.com/Article/details/guricdmzs.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.hesvh.cn/Article/details/gruigujng.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.zdbjq.cn/Article/details/glmhbgwhf.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.hesvh.cn/Article/details/gccakxgeq.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.zdbjq.cn/Article/details/galmbywtn.sHtML

[T08] Kotlin：数据类
来源：http://www.share.zdbjq.cn/Article/details/gcxmempsq.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.hesvh.cn/Article/details/gdklnekld.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.fehbvm.com/Article/details/gjjertffg.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.fehbvm.com/Article/details/gictnzoxm.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.hesvh.cn/Article/details/gqyhdmkey.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.zdbjq.cn/Article/details/guetpbppg.sHtML

[T11] Kotlin：协程
来源：http://baike.hesvh.cn/Article/details/gfqtvzbcy.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.zdbjq.cn/Article/details/gidgzzytq.sHtML

[T12] Kotlin：解构声明
来源：http://wap.fehbvm.com/Article/details/gqinjqked.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.hesvh.cn/Article/details/gutvoqpgt.sHtML


<!-- 参考信息 -->