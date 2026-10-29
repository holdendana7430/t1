代发 wailian999

for i in {1..10}; do echo "$i"; done
来源：http://read.share.hesvh.cn/Article/details/gntayhcxo.sHtML

[R14] C 风格 for
来源：http://m.share.hesvh.cn/Article/details/gwjfenwqs.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.fehbvm.com/Article/details/gudmlxcvm.sHtML

[R15] while 逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gpketvljw.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.fehbvm.com/Article/details/gmaxqnbri.sHtML

[R16] until 等待条件
来源：http://wap.zdbjq.cn/Article/details/gayjeakxe.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.zdbjq.cn/Article/details/gnpumpcws.sHtML

[R17] 数组定义与取值
来源：http://read.share.zdbjq.cn/Article/details/geivbjbbn.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.zdbjq.cn/Article/details/gpjqtfknn.sHtML

[R18] 遍历数组
来源：http://wap.hesvh.cn/Article/details/gbncovain.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.fehbvm.com/Article/details/gbtzscmoq.sHtML

[R19] 数组长度
来源：http://read.share.hesvh.cn/Article/details/gsbullbfs.sHtML

echo "${#arr[@]}"
来源：http://blog.zdbjq.cn/Article/details/gcchnyknr.sHtML

[R20] 关联数组（字典）
来源：http://m.share.fehbvm.com/Article/details/gxpuppvxd.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.fehbvm.com/Article/details/gqwzpnipl.sHtML

[R21] 字符串长度
来源：http://m.share.zdbjq.cn/Article/details/gnpwnpxqa.sHtML

echo "${#s}"
来源：http://mobile.zdbjq.cn/Article/details/gkwxjvpwa.sHtML

[R22] 截取子串
来源：http://3g.fehbvm.com/Article/details/gofipigtp.sHtML

echo "${s:0:5}"
来源：http://mobile.hesvh.cn/Article/details/gofjokqeu.sHtML

[R23] 字符串替换
来源：http://blog.fehbvm.com/Article/details/ggelxirhg.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.zdbjq.cn/Article/details/gpoftwfbt.sHtML

[R24] 大小写转换
来源：http://www.m.share.fehbvm.com/Article/details/gatoodlms.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.hesvh.cn/Article/details/gvefzxaay.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.hesvh.cn/Article/details/gmljzvvjo.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.hesvh.cn/Article/details/grxdqujph.sHtML

[R26] 命令替换
来源：http://3g.hesvh.cn/Article/details/gtrtybksq.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.zdbjq.cn/Article/details/glajxsomn.sHtML

[R27] 算术展开
来源：http://www.share.hesvh.cn/Article/details/gfrdhzdqa.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.hesvh.cn/Article/details/guxupuvbn.sHtML

[R28] 浮点运算
来源：http://www.m.share.fehbvm.com/Article/details/gkmyklegv.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.zdbjq.cn/Article/details/gsjgfyrgc.sHtML

[R29] 定义函数
来源：http://www.blog.fehbvm.com/Article/details/gnnmnildz.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fehbvm.com/Article/details/gkjlemnzq.sHtML

[R30] 函数返回状态码
来源：http://wap.fehbvm.com/Article/details/gfkojhydn.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.zdbjq.cn/Article/details/ggdqjfkpa.sHtML

[R31] 局部变量
来源：http://blog.hesvh.cn/Article/details/gpopsmxgg.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fehbvm.com/Article/details/gdvylbeqe.sHtML

[R32] 参数个数校验
来源：http://mobile.zdbjq.cn/Article/details/gndshsmry.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.fehbvm.com/Article/details/gwfiranxc.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fehbvm.com/Article/details/gvdzfdgpq.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.fehbvm.com/Article/details/gusllahma.sHtML

[R34] 退出时清理
来源：http://www.m.share.hesvh.cn/Article/details/gjhfobdhx.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.hesvh.cn/Article/details/grbbtykme.sHtML

[R35] 后台执行并等待
来源：http://wap.hesvh.cn/Article/details/gadxrjnpj.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fehbvm.com/Article/details/gnuujmwcf.sHtML

[R36] 并发执行多个任务
来源：http://read.share.hesvh.cn/Article/details/gkpkajumm.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.zdbjq.cn/Article/details/gadrpexqh.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.zdbjq.cn/Article/details/grygyvuat.sHtML

files=$(ls -1)
来源：http://m.share.fehbvm.com/Article/details/gzrbxcxcw.sHtML

[R38] 管道串联
来源：http://baike.zdbjq.cn/Article/details/guvnbtgka.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.zdbjq.cn/Article/details/gbtjdmizv.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.fehbvm.com/Article/details/gvnausklr.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.hesvh.cn/Article/details/gvjfmhbwc.sHtML

[R40] 追加写日志
来源：http://www.m.share.zdbjq.cn/Article/details/gqwicwzqt.sHtML

echo "log" >> out.log
来源：http://m.share.fehbvm.com/Article/details/gxejpsrwd.sHtML

[R41] 丢弃输出
来源：http://www.m.share.zdbjq.cn/Article/details/gotulgezg.sHtML

cmd >/dev/null 2>&1
来源：http://blog.fehbvm.com/Article/details/gtehfobjl.sHtML

[R42] 输入重定向
来源：http://wap.fehbvm.com/Article/details/grumrnviw.sHtML

wc -l < a.txt
来源：http://read.share.fehbvm.com/Article/details/gwdexbodp.sHtML

[R43] 按名字查找文件
来源：http://blog.fehbvm.com/Article/details/gsojbqbuq.sHtML

find . -name "*.log" -type f
来源：http://blog.hesvh.cn/Article/details/gekjkbaoi.sHtML

[R44] 按修改时间查找
来源：http://blog.zdbjq.cn/Article/details/gkpqapvny.sHtML

find . -mtime -7 -type f
来源：http://3g.zdbjq.cn/Article/details/gnmvctuhe.sHtML

[R45] 批量删除
来源：http://www.share.hesvh.cn/Article/details/guyzxaokc.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.fehbvm.com/Article/details/gfhxeuori.sHtML

[R46] 递归替换文件内容
来源：http://mobile.zdbjq.cn/Article/details/gcjeevfak.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fehbvm.com/Article/details/gcqsjnggv.sHtML

[R47] sed 单行替换
来源：http://www.m.share.hesvh.cn/Article/details/ghoddaxzg.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.hesvh.cn/Article/details/gnzhgiteh.sHtML

[R48] awk 取指定列
来源：http://www.m.share.hesvh.cn/Article/details/gqyoqclcq.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.zdbjq.cn/Article/details/gonpqkzjy.sHtML

[R49] awk 带条件
来源：http://m.share.fehbvm.com/Article/details/gwiwvdtvd.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fehbvm.com/Article/details/gotbbypcw.sHtML

[R50] awk 求和
来源：http://www.blog.hesvh.cn/Article/details/gkhkxbtck.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fehbvm.com/Article/details/ghvpoqdyd.sHtML

[R51] 排序去重取前几
来源：http://mobile.hesvh.cn/Article/details/gdmemzzmz.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.hesvh.cn/Article/details/glcgdagfd.sHtML

[R52] 统计行数
来源：http://mobile.zdbjq.cn/Article/details/gxrejvugv.sHtML

wc -l a.txt
来源：http://www.blog.fehbvm.com/Article/details/gpmqfwhjb.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.zdbjq.cn/Article/details/ggfoudjvw.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.zdbjq.cn/Article/details/gyoyrlvje.sHtML

[R54] 比较两个文件
来源：http://blog.hesvh.cn/Article/details/giyofbdac.sHtML

diff a.txt b.txt
来源：http://www.blog.zdbjq.cn/Article/details/ggunrjwgo.sHtML

[R55] 压缩与解压
来源：http://www.share.fehbvm.com/Article/details/gfmyulhgl.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.zdbjq.cn/Article/details/gqdsfjbbb.sHtML

[R56] 远程拷贝
来源：http://www.blog.hesvh.cn/Article/details/gvmaflvul.sHtML

scp file user@host:/path/
来源：http://www.blog.zdbjq.cn/Article/details/gdmswwbci.sHtML

[R57] 远程执行命令
来源：http://3g.fehbvm.com/Article/details/gxlrkxgcs.sHtML

ssh user@host 'uptime'
来源：http://blog.fehbvm.com/Article/details/gxewbwmnj.sHtML

[R58] 下载文件
来源：http://3g.fehbvm.com/Article/details/ghhiqliak.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.zdbjq.cn/Article/details/gffretves.sHtML

[R59] 发 POST JSON
来源：http://www.share.fehbvm.com/Article/details/gupqtnsve.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.hesvh.cn/Article/details/gcwmgvabn.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fehbvm.com/Article/details/gozgfpzgr.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.fehbvm.com/Article/details/glpdwyugq.sHtML

[R61] 磁盘占用
来源：http://3g.hesvh.cn/Article/details/gfdykzjzz.sHtML

df -h;  du -sh *
来源：http://mobile.fehbvm.com/Article/details/gzjtqrndm.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fehbvm.com/Article/details/glhjtvyng.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fehbvm.com/Article/details/garqqfadn.sHtML

[R63] 内存与进程
来源：http://www.share.hesvh.cn/Article/details/glhtfeord.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.zdbjq.cn/Article/details/gsdwwhxoo.sHtML

[R64] 结束进程
来源：http://www.m.share.fehbvm.com/Article/details/gnsolaawh.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.hesvh.cn/Article/details/gxgjeilkj.sHtML

[R65] 查看端口占用
来源：http://read.share.hesvh.cn/Article/details/gsoositoh.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.hesvh.cn/Article/details/gdwjyghab.sHtML

[R66] 定时任务
来源：http://www.blog.hesvh.cn/Article/details/gljdpwwpo.sHtML

crontab -e;  crontab -l
来源：http://3g.fehbvm.com/Article/details/ghtghxirq.sHtML

[R67] 生成随机十六进制串
来源：http://3g.hesvh.cn/Article/details/giezyrtzt.sHtML

openssl rand -hex 16
来源：http://www.m.share.hesvh.cn/Article/details/gflgnitxf.sHtML

[R68] 计算文件校验值
来源：http://m.share.fehbvm.com/Article/details/gqjnnaykp.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.zdbjq.cn/Article/details/gnxghtqsk.sHtML

[R69] 生成随机密码
来源：http://blog.zdbjq.cn/Article/details/gseqheevr.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.zdbjq.cn/Article/details/gjeduoaoy.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.zdbjq.cn/Article/details/gmjzsyhyv.sHtML

date +%s;  date -d @1700000000
来源：http://baike.zdbjq.cn/Article/details/gejawmejj.sHtML

[R71] 日期格式化
来源：http://baike.zdbjq.cn/Article/details/gleihibyg.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fehbvm.com/Article/details/gssidofbk.sHtML

[R72] 等待端口就绪
来源：http://3g.zdbjq.cn/Article/details/gvwajtzcd.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fehbvm.com/Article/details/gznxfaziw.sHtML

[R73] 分割大日志
来源：http://baike.zdbjq.cn/Article/details/gfzjounzk.sHtML

split -l 1000 big.log part_
来源：http://blog.hesvh.cn/Article/details/gbwlvqite.sHtML

[R74] 批量重命名
来源：http://wap.hesvh.cn/Article/details/glqzggfgf.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.hesvh.cn/Article/details/gfquajnyy.sHtML

[R75] 导出环境变量
来源：http://www.m.share.hesvh.cn/Article/details/gngjuaoxy.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.zdbjq.cn/Article/details/gohgndivs.sHtML

[R76] 使用临时文件
来源：http://blog.zdbjq.cn/Article/details/ggtrxwbbw.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.zdbjq.cn/Article/details/gguoovdmh.sHtML

[R77] 读取用户输入
来源：http://www.share.fehbvm.com/Article/details/gpywknzps.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fehbvm.com/Article/details/gvsmjtxkw.sHtML

[R78] 交互式菜单
来源：http://www.m.share.fehbvm.com/Article/details/gvhnbzvpf.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.hesvh.cn/Article/details/gszaayjif.sHtML

[R79] 解析命令行选项
来源：http://read.share.fehbvm.com/Article/details/grviqispr.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.zdbjq.cn/Article/details/gmpiuavbe.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.fehbvm.com/Article/details/gdyawpqjv.sHtML

time ./run.sh
来源：http://m.share.zdbjq.cn/Article/details/gihamstmd.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/guffkteta.sHtML

S. C / C++ 专题
来源：http://wap.zdbjq.cn/Article/details/gaishcrbl.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gwmlstfeo.sHtML

[S01] C：Hello World
来源：http://mobile.hesvh.cn/Article/details/gbjqbscmp.sHtML

#include <stdio.h>
来源：http://wap.zdbjq.cn/Article/details/gqbvkhdxd.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.hesvh.cn/Article/details/gwziuzhzh.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.zdbjq.cn/Article/details/gzogdysoj.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fehbvm.com/Article/details/gyjgpzwgu.sHtML

[S03] C：读入整数
来源：http://www.m.share.fehbvm.com/Article/details/gmapkmdrn.sHtML

int x; scanf("%d", &x);
来源：http://wap.hesvh.cn/Article/details/gmbrsqkmu.sHtML

[S04] C：字符串复制
来源：http://baike.fehbvm.com/Article/details/gmnqlvxao.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.fehbvm.com/Article/details/goqfjahwy.sHtML

[S05] C：字符串长度
来源：http://www.blog.hesvh.cn/Article/details/gdihivjnb.sHtML

strlen(s)
来源：http://www.blog.hesvh.cn/Article/details/gwxlscmxg.sHtML

[S06] C：字符串比较
来源：http://wap.fehbvm.com/Article/details/gnhszynfd.sHtML

strcmp(a, b) == 0
来源：http://baike.hesvh.cn/Article/details/gnezqnwtn.sHtML

[S07] C：数组遍历求和
来源：http://3g.zdbjq.cn/Article/details/gwjsbtilz.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.hesvh.cn/Article/details/gvmuhjmxv.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fehbvm.com/Article/details/grjpwvrgp.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.zdbjq.cn/Article/details/gyahzaqjx.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fehbvm.com/Article/details/grrglciym.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.fehbvm.com/Article/details/gtextcwij.sHtML

[S10] C：指针与解引用
来源：http://mobile.hesvh.cn/Article/details/ghotfeyzx.sHtML

int *p = &a;  *p = 5;
来源：http://blog.zdbjq.cn/Article/details/gvniogojd.sHtML

[S11] C：逐行读文件
来源：http://wap.fehbvm.com/Article/details/geetijegt.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.zdbjq.cn/Article/details/gwhedejht.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.hesvh.cn/Article/details/gwcijrkhq.sHtML

fclose(f);
来源：http://wap.zdbjq.cn/Article/details/gsivqtmjy.sHtML

[S12] C：写文件
来源：http://www.share.hesvh.cn/Article/details/grcqjnaxh.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.hesvh.cn/Article/details/gioxdxtgj.sHtML

[S13] C：宏定义
来源：http://www.share.zdbjq.cn/Article/details/gunjjqfbj.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.hesvh.cn/Article/details/gfpugdfky.sHtML

[S14] C：枚举
来源：http://baike.hesvh.cn/Article/details/gwnacqiex.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.fehbvm.com/Article/details/giivnibfb.sHtML

[S15] C：类型转换
来源：http://www.m.share.zdbjq.cn/Article/details/gjuvlozxh.sHtML

(double) a / b
来源：http://mobile.zdbjq.cn/Article/details/gmacoxmab.sHtML

[S16] C：位操作置位
来源：http://mobile.fehbvm.com/Article/details/gieeerias.sHtML

x |= (1 << 3);
来源：http://mobile.hesvh.cn/Article/details/gtywrcskh.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/gzpcpvcjk.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.hesvh.cn/Article/details/gtqdjcbvy.sHtML

[S18] C：命令行参数
来源：http://m.share.hesvh.cn/Article/details/gegxuyeen.sHtML

int main(int argc, char **argv)
来源：http://mobile.zdbjq.cn/Article/details/ggmsyhidb.sHtML

[S19] C：快速排序
来源：http://blog.hesvh.cn/Article/details/gbsjjeavu.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fehbvm.com/Article/details/gwjorhhxm.sHtML

[S20] C：二分查找
来源：http://read.share.zdbjq.cn/Article/details/gcpxajrwe.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.zdbjq.cn/Article/details/giatffpov.sHtML

[S21] C：字符类别判断
来源：http://m.share.fehbvm.com/Article/details/gjjdehfrn.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.zdbjq.cn/Article/details/gnzcxwexy.sHtML

[S22] C：字符串转数字
来源：http://3g.zdbjq.cn/Article/details/gthzcaihr.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.hesvh.cn/Article/details/gzvzqwjpo.sHtML

[S23] C：随机数
来源：http://3g.zdbjq.cn/Article/details/gckqrcprv.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.zdbjq.cn/Article/details/gujzkmfsw.sHtML

[S24] C：获取本地时间
来源：http://www.blog.hesvh.cn/Article/details/gilfrvcpg.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.hesvh.cn/Article/details/gsfvurcck.sHtML

[S25] C：内存拷贝
来源：http://blog.hesvh.cn/Article/details/gdivqkxsb.sHtML

memcpy(dst, src, n);
来源：http://www.share.zdbjq.cn/Article/details/ghkxcgprp.sHtML

[S26] C：内存清零
来源：http://3g.hesvh.cn/Article/details/gaywbpiqb.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.zdbjq.cn/Article/details/gowpohvia.sHtML

[S27] C：定义常量
来源：http://mobile.hesvh.cn/Article/details/ghtumbnyn.sHtML

const double PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gamvaqxsv.sHtML

[S28] C：静态变量
来源：http://www.blog.zdbjq.cn/Article/details/gknblilim.sHtML

static int counter = 0;
来源：http://www.m.share.hesvh.cn/Article/details/gsnrdlinp.sHtML

[S29] C：变参函数
来源：http://3g.hesvh.cn/Article/details/ghpogpwgt.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.zdbjq.cn/Article/details/gnmgxqsci.sHtML

[S30] C：头文件保护
来源：http://wap.hesvh.cn/Article/details/gjmtcqgrp.sHtML

#ifndef X_H
来源：http://www.blog.fehbvm.com/Article/details/gobfbcdyr.sHtML

#define X_H
来源：http://3g.fehbvm.com/Article/details/gcortsgcq.sHtML

#endif
来源：http://wap.fehbvm.com/Article/details/gqxuyoomg.sHtML

[S31] C++：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gyfxfjqqu.sHtML

#include <iostream>
来源：http://baike.fehbvm.com/Article/details/gdgvplysz.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fehbvm.com/Article/details/gzcntdjtv.sHtML

[S32] C++：字符串
来源：http://www.blog.fehbvm.com/Article/details/gywxlnzdd.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.hesvh.cn/Article/details/gfigikzvb.sHtML

[S33] C++：vector 增删
来源：http://mobile.hesvh.cn/Article/details/ghnuxwemw.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.zdbjq.cn/Article/details/gblqurtgl.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.hesvh.cn/Article/details/giyrsbyri.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.hesvh.cn/Article/details/gynpsjskj.sHtML

[S35] C++：map
来源：http://baike.hesvh.cn/Article/details/gxyptnwzj.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gzyytlini.sHtML

[S36] C++：unordered_map
来源：http://m.share.fehbvm.com/Article/details/gbpoupibj.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/geqvexteb.sHtML

[S37] C++：set
来源：http://www.share.fehbvm.com/Article/details/gxexzgszt.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.hesvh.cn/Article/details/gaiorpewi.sHtML

[S38] C++：排序
来源：http://baike.hesvh.cn/Article/details/grxnholpc.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fehbvm.com/Article/details/gdoqjmlnj.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.hesvh.cn/Article/details/gqbwaftsp.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.zdbjq.cn/Article/details/givzrwlow.sHtML

[S40] C++：查找元素
来源：http://wap.hesvh.cn/Article/details/ggodpryex.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.hesvh.cn/Article/details/gbfryklmm.sHtML

[S41] C++：类与构造函数
来源：http://www.share.fehbvm.com/Article/details/gmvgtighg.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.fehbvm.com/Article/details/gacmjtpqs.sHtML

[S42] C++：继承与虚函数
来源：http://wap.fehbvm.com/Article/details/giokwtkbm.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.fehbvm.com/Article/details/gfyszlurt.sHtML

[S43] C++：智能指针
来源：http://blog.zdbjq.cn/Article/details/gjjwrwqti.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.hesvh.cn/Article/details/golrvpbfe.sHtML

[S44] C++：引用传参
来源：http://blog.zdbjq.cn/Article/details/gmjcyhqff.sHtML

void inc(int &x) { ++x; }
来源：http://baike.fehbvm.com/Article/details/gugxotmcu.sHtML

[S45] C++：lambda
来源：http://www.blog.hesvh.cn/Article/details/gaczkrrvv.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.fehbvm.com/Article/details/glqmzkgpb.sHtML

[S46] C++：函数模板
来源：http://wap.hesvh.cn/Article/details/goncxnxcv.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.fehbvm.com/Article/details/gomecnofr.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.fehbvm.com/Article/details/gceajidcv.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.fehbvm.com/Article/details/ghesrgzxv.sHtML

[S48] C++：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gdeaovori.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.fehbvm.com/Article/details/grgbvqvhl.sHtML

while (std::getline(in, line)) { }
来源：http://3g.hesvh.cn/Article/details/gchrnojsx.sHtML

[S49] C++：写文件
来源：http://baike.fehbvm.com/Article/details/gtjmyiwcx.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.zdbjq.cn/Article/details/gsdpiroke.sHtML

[S50] C++：格式化数字
来源：http://mobile.zdbjq.cn/Article/details/glwxdlyom.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gfzpayphg.sHtML

[S51] C++：显式类型转换
来源：http://3g.hesvh.cn/Article/details/gfwwuvljg.sHtML

static_cast<double>(a) / b
来源：http://baike.hesvh.cn/Article/details/gneffldng.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.zdbjq.cn/Article/details/gmcewdypl.sHtML

int size() const noexcept { return n_; }
来源：http://3g.fehbvm.com/Article/details/ggzihjmzc.sHtML

[S53] C++：移动语义
来源：http://baike.hesvh.cn/Article/details/gsxzbcsvu.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.fehbvm.com/Article/details/gukgnzmdl.sHtML

[S54] C++：异常处理
来源：http://3g.hesvh.cn/Article/details/gxzynlvcp.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.hesvh.cn/Article/details/gzcneobxu.sHtML

[S55] C++：结构化绑定
来源：http://3g.zdbjq.cn/Article/details/gbtiblgeu.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.fehbvm.com/Article/details/gvnwyergm.sHtML

[S56] C++：optional
来源：http://m.share.hesvh.cn/Article/details/gwvwwtmht.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.fehbvm.com/Article/details/gmxpxweeo.sHtML

[S57] C++：编译期常量
来源：http://wap.zdbjq.cn/Article/details/gegruqnii.sHtML

constexpr int N = 10;
来源：http://mobile.hesvh.cn/Article/details/gltrohvdg.sHtML

[S58] C++：命名空间
来源：http://wap.hesvh.cn/Article/details/ghoquubkh.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.zdbjq.cn/Article/details/gdxqjkuiy.sHtML

[S59] C++：静态断言
来源：http://baike.fehbvm.com/Article/details/gmdtxixov.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.hesvh.cn/Article/details/gzraloekl.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.fehbvm.com/Article/details/gzsbpvtkf.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.hesvh.cn/Article/details/gokvixtuf.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gdqkffnfj.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.zdbjq.cn/Article/details/gcrldrycm.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gamyttiqa.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gurysereq.sHtML

println("Hello")
来源：http://blog.zdbjq.cn/Article/details/gknxkbqif.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.zdbjq.cn/Article/details/goovtxgxn.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.hesvh.cn/Article/details/gbrmzlofz.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.zdbjq.cn/Article/details/giqroloty.sHtML

"值: $b"
来源：http://m.share.hesvh.cn/Article/details/gihbsolkl.sHtML

[T04] Kotlin：空安全
来源：http://m.share.fehbvm.com/Article/details/gfugkvioz.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.zdbjq.cn/Article/details/gfkwzrsfc.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.fehbvm.com/Article/details/gicolzqyo.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.fehbvm.com/Article/details/gbpjhmupw.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.hesvh.cn/Article/details/gxlvyzkyn.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.hesvh.cn/Article/details/gxkszrdpm.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.hesvh.cn/Article/details/gzswfsjql.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.zdbjq.cn/Article/details/guantasyr.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.fehbvm.com/Article/details/gttakbuay.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.zdbjq.cn/Article/details/gkrlypplu.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.hesvh.cn/Article/details/gvguxybse.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.zdbjq.cn/Article/details/gfwwojmhu.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.zdbjq.cn/Article/details/guvwrtpsv.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.hesvh.cn/Article/details/gnohjxqtu.sHtML

[T11] Kotlin：协程
来源：http://wap.hesvh.cn/Article/details/gzsnqvzrp.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.zdbjq.cn/Article/details/gegyujrkd.sHtML

[T12] Kotlin：解构声明
来源：http://3g.fehbvm.com/Article/details/giiufovwk.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gcfmwevxn.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.fehbvm.com/Article/details/gkceouvdm.sHtML

val m = mapOf("a" to 1)
来源：http://blog.zdbjq.cn/Article/details/gehkkiyzy.sHtML

[T14] Kotlin：循环
来源：http://read.share.fehbvm.com/Article/details/gmtuavowa.sHtML

for (i in 1..10) println(i)
来源：http://mobile.zdbjq.cn/Article/details/gpmdymagv.sHtML

[T15] Kotlin：接口
来源：http://www.share.fehbvm.com/Article/details/gdaynxffl.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.fehbvm.com/Article/details/gjnbuyjmv.sHtML

[T16] Swift：Hello World
来源：http://m.share.hesvh.cn/Article/details/gkadvfono.sHtML

print("Hello")
来源：http://blog.hesvh.cn/Article/details/gptunymbq.sHtML


<!-- 参考信息 -->