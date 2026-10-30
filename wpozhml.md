代发 wailian999

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.fehbvm.com/Article/details/gmjmtvhlr.sHtML

[R18] 遍历数组
来源：http://www.m.share.hesvh.cn/Article/details/gmytisbpb.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.zdbjq.cn/Article/details/gvuinjygp.sHtML

[R19] 数组长度
来源：http://www.m.share.hesvh.cn/Article/details/gjlkrkwsi.sHtML

echo "${#arr[@]}"
来源：http://baike.zdbjq.cn/Article/details/gcpcbnhoi.sHtML

[R20] 关联数组（字典）
来源：http://m.share.fehbvm.com/Article/details/gxnxthsvd.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.fehbvm.com/Article/details/gxjhzfksb.sHtML

[R21] 字符串长度
来源：http://3g.fehbvm.com/Article/details/gmsngdyix.sHtML

echo "${#s}"
来源：http://blog.zdbjq.cn/Article/details/gqqhokntm.sHtML

[R22] 截取子串
来源：http://m.share.fehbvm.com/Article/details/gguakmrhi.sHtML

echo "${s:0:5}"
来源：http://mobile.hesvh.cn/Article/details/gkgqktrnf.sHtML

[R23] 字符串替换
来源：http://wap.hesvh.cn/Article/details/gqclgaviy.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.zdbjq.cn/Article/details/gyghoubsc.sHtML

[R24] 大小写转换
来源：http://www.m.share.zdbjq.cn/Article/details/grvzubffz.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fehbvm.com/Article/details/gbnrfthrp.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.hesvh.cn/Article/details/gytbziumt.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.zdbjq.cn/Article/details/gdjvuavdp.sHtML

[R26] 命令替换
来源：http://blog.fehbvm.com/Article/details/gqjoafbga.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.hesvh.cn/Article/details/gqguzpztl.sHtML

[R27] 算术展开
来源：http://read.share.hesvh.cn/Article/details/gdusmrhnk.sHtML

echo $((1 + 2 * 3))
来源：http://blog.hesvh.cn/Article/details/gmijqyikj.sHtML

[R28] 浮点运算
来源：http://wap.hesvh.cn/Article/details/gkcwckpxz.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.zdbjq.cn/Article/details/guucivsas.sHtML

[R29] 定义函数
来源：http://www.m.share.fehbvm.com/Article/details/gnrddbxho.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.hesvh.cn/Article/details/grribfegq.sHtML

[R30] 函数返回状态码
来源：http://blog.hesvh.cn/Article/details/gzmlgofqe.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.hesvh.cn/Article/details/gstcfegzs.sHtML

[R31] 局部变量
来源：http://mobile.zdbjq.cn/Article/details/gmqapacxt.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.hesvh.cn/Article/details/gtqdyksda.sHtML

[R32] 参数个数校验
来源：http://www.blog.fehbvm.com/Article/details/gozmlodpa.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.fehbvm.com/Article/details/gcygduqyf.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.hesvh.cn/Article/details/gbrbwwewg.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.zdbjq.cn/Article/details/gfqulksvc.sHtML

[R34] 退出时清理
来源：http://www.share.fehbvm.com/Article/details/glxqcirbr.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.fehbvm.com/Article/details/guumurquv.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fehbvm.com/Article/details/gwvmuvyfb.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.fehbvm.com/Article/details/gtegysjpo.sHtML

[R36] 并发执行多个任务
来源：http://mobile.zdbjq.cn/Article/details/grohubyhk.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.hesvh.cn/Article/details/gfcwkcdrw.sHtML

[R37] 把输出赋给变量
来源：http://blog.hesvh.cn/Article/details/gwmlhyast.sHtML

files=$(ls -1)
来源：http://blog.hesvh.cn/Article/details/gkaaakfmo.sHtML

[R38] 管道串联
来源：http://www.m.share.hesvh.cn/Article/details/gwxplniuq.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.zdbjq.cn/Article/details/gopuxynjz.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.hesvh.cn/Article/details/gfosfovxr.sHtML

cmd > out.log 2>&1
来源：http://wap.fehbvm.com/Article/details/gbytrcotj.sHtML

[R40] 追加写日志
来源：http://baike.zdbjq.cn/Article/details/gpdqbcqhh.sHtML

echo "log" >> out.log
来源：http://www.m.share.zdbjq.cn/Article/details/gmncyaiwl.sHtML

[R41] 丢弃输出
来源：http://www.m.share.hesvh.cn/Article/details/gfhybwylz.sHtML

cmd >/dev/null 2>&1
来源：http://3g.hesvh.cn/Article/details/gxnjvqoui.sHtML

[R42] 输入重定向
来源：http://blog.hesvh.cn/Article/details/gylpdylqa.sHtML

wc -l < a.txt
来源：http://www.blog.fehbvm.com/Article/details/gcoqzvskl.sHtML

[R43] 按名字查找文件
来源：http://mobile.zdbjq.cn/Article/details/gdbqcgymg.sHtML

find . -name "*.log" -type f
来源：http://www.share.fehbvm.com/Article/details/gkbpvkxpm.sHtML

[R44] 按修改时间查找
来源：http://www.share.hesvh.cn/Article/details/gmnidfgfm.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fehbvm.com/Article/details/gzbriance.sHtML

[R45] 批量删除
来源：http://m.share.zdbjq.cn/Article/details/gangrmegn.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.hesvh.cn/Article/details/gycouazef.sHtML

[R46] 递归替换文件内容
来源：http://wap.zdbjq.cn/Article/details/giapretcg.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.zdbjq.cn/Article/details/gscofxgmt.sHtML

[R47] sed 单行替换
来源：http://blog.fehbvm.com/Article/details/gjuymuexd.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.zdbjq.cn/Article/details/gbjrlihrd.sHtML

[R48] awk 取指定列
来源：http://www.m.share.hesvh.cn/Article/details/gbkemngsn.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.hesvh.cn/Article/details/gcqfguylh.sHtML

[R49] awk 带条件
来源：http://blog.zdbjq.cn/Article/details/glspaviec.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.hesvh.cn/Article/details/gfxlywwoc.sHtML

[R50] awk 求和
来源：http://baike.fehbvm.com/Article/details/guiodhcyv.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.zdbjq.cn/Article/details/gsvuqcmvz.sHtML

[R51] 排序去重取前几
来源：http://baike.hesvh.cn/Article/details/giuycarhm.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.hesvh.cn/Article/details/gcrtvlqus.sHtML

[R52] 统计行数
来源：http://www.share.hesvh.cn/Article/details/ganrhfbfc.sHtML

wc -l a.txt
来源：http://m.share.hesvh.cn/Article/details/gkwmoxnai.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.fehbvm.com/Article/details/gexzyjaai.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.zdbjq.cn/Article/details/gpywefacm.sHtML

[R54] 比较两个文件
来源：http://mobile.hesvh.cn/Article/details/ghkmosihv.sHtML

diff a.txt b.txt
来源：http://www.blog.fehbvm.com/Article/details/gwlxgwymq.sHtML

[R55] 压缩与解压
来源：http://blog.fehbvm.com/Article/details/gpdecifaq.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.hesvh.cn/Article/details/gysminjgm.sHtML

[R56] 远程拷贝
来源：http://mobile.fehbvm.com/Article/details/guqlkxkdc.sHtML

scp file user@host:/path/
来源：http://baike.fehbvm.com/Article/details/gidfaqoje.sHtML

[R57] 远程执行命令
来源：http://www.share.hesvh.cn/Article/details/gniwqnaeq.sHtML

ssh user@host 'uptime'
来源：http://blog.fehbvm.com/Article/details/ghcoimjrv.sHtML

[R58] 下载文件
来源：http://m.share.hesvh.cn/Article/details/grxntoavx.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.zdbjq.cn/Article/details/gjmttzhzj.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.zdbjq.cn/Article/details/gukdicapx.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.hesvh.cn/Article/details/gwjvrwnms.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fehbvm.com/Article/details/gpjbghxqq.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.hesvh.cn/Article/details/gnvciuzqx.sHtML

[R61] 磁盘占用
来源：http://baike.zdbjq.cn/Article/details/gswvoujod.sHtML

df -h;  du -sh *
来源：http://www.m.share.zdbjq.cn/Article/details/gbsrcbkwq.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.zdbjq.cn/Article/details/gvhiyytey.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.hesvh.cn/Article/details/geewdzcsr.sHtML

[R63] 内存与进程
来源：http://baike.zdbjq.cn/Article/details/gbraeczqx.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.zdbjq.cn/Article/details/gtwdjfruz.sHtML

[R64] 结束进程
来源：http://wap.hesvh.cn/Article/details/gptqirwgu.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.hesvh.cn/Article/details/gnaktalxt.sHtML

[R65] 查看端口占用
来源：http://www.blog.zdbjq.cn/Article/details/gqdqzhznq.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.hesvh.cn/Article/details/gxfsmnswo.sHtML

[R66] 定时任务
来源：http://wap.fehbvm.com/Article/details/gyykjqaob.sHtML

crontab -e;  crontab -l
来源：http://www.share.hesvh.cn/Article/details/gvsmwwoxz.sHtML

[R67] 生成随机十六进制串
来源：http://3g.zdbjq.cn/Article/details/gyrsuljfd.sHtML

openssl rand -hex 16
来源：http://read.share.fehbvm.com/Article/details/gxgucdxyb.sHtML

[R68] 计算文件校验值
来源：http://www.share.zdbjq.cn/Article/details/gdjdnmaee.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.hesvh.cn/Article/details/gynhtxipi.sHtML

[R69] 生成随机密码
来源：http://3g.fehbvm.com/Article/details/gwpitonoy.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.hesvh.cn/Article/details/gjxuieogw.sHtML

[R70] 时间戳与互转
来源：http://read.share.hesvh.cn/Article/details/grkssnvhi.sHtML

date +%s;  date -d @1700000000
来源：http://blog.fehbvm.com/Article/details/grynnyluo.sHtML

[R71] 日期格式化
来源：http://read.share.hesvh.cn/Article/details/gdblxfsuk.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.zdbjq.cn/Article/details/gufyqotbv.sHtML

[R72] 等待端口就绪
来源：http://www.share.zdbjq.cn/Article/details/ghbydkrqs.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.hesvh.cn/Article/details/gfkpuqnnc.sHtML

[R73] 分割大日志
来源：http://3g.zdbjq.cn/Article/details/gpgrzadqo.sHtML

split -l 1000 big.log part_
来源：http://baike.fehbvm.com/Article/details/ggkbmyogj.sHtML

[R74] 批量重命名
来源：http://www.blog.zdbjq.cn/Article/details/gxuwxmlvb.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gdsehuzmv.sHtML

[R75] 导出环境变量
来源：http://www.blog.hesvh.cn/Article/details/gwsakoebx.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.fehbvm.com/Article/details/gltefjxls.sHtML

[R76] 使用临时文件
来源：http://3g.fehbvm.com/Article/details/gegzjvkcn.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.hesvh.cn/Article/details/gkizpyijj.sHtML

[R77] 读取用户输入
来源：http://www.share.hesvh.cn/Article/details/geaqwxsjw.sHtML

read -rp "请输入: " ans
来源：http://m.share.hesvh.cn/Article/details/gfudfoprc.sHtML

[R78] 交互式菜单
来源：http://mobile.fehbvm.com/Article/details/gayefevlw.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.zdbjq.cn/Article/details/gjaarzlqo.sHtML

[R79] 解析命令行选项
来源：http://baike.hesvh.cn/Article/details/genawqelz.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.zdbjq.cn/Article/details/gvjlecxsb.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fehbvm.com/Article/details/gxrtxferr.sHtML

time ./run.sh
来源：http://mobile.fehbvm.com/Article/details/glxrcwunz.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gagwbkhqo.sHtML

S. C / C++ 专题
来源：http://3g.hesvh.cn/Article/details/ghecmbvge.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/giieehxai.sHtML

[S01] C：Hello World
来源：http://wap.hesvh.cn/Article/details/gbwoghkuo.sHtML

#include <stdio.h>
来源：http://www.share.hesvh.cn/Article/details/gkolgevkg.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.fehbvm.com/Article/details/gseskqtfx.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.zdbjq.cn/Article/details/ghalfuxpq.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.hesvh.cn/Article/details/gryortpkp.sHtML

[S03] C：读入整数
来源：http://www.m.share.hesvh.cn/Article/details/gcdrkwrmu.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.fehbvm.com/Article/details/gklubddfn.sHtML

[S04] C：字符串复制
来源：http://3g.fehbvm.com/Article/details/gzofcgwzs.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.hesvh.cn/Article/details/ghplqeius.sHtML

[S05] C：字符串长度
来源：http://www.m.share.zdbjq.cn/Article/details/gracvbknv.sHtML

strlen(s)
来源：http://3g.fehbvm.com/Article/details/gfswzurzf.sHtML

[S06] C：字符串比较
来源：http://blog.hesvh.cn/Article/details/gfvcbhxtd.sHtML

strcmp(a, b) == 0
来源：http://3g.zdbjq.cn/Article/details/guzqdpned.sHtML

[S07] C：数组遍历求和
来源：http://mobile.fehbvm.com/Article/details/gzjrkgcyp.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.hesvh.cn/Article/details/gplrlzrmg.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.zdbjq.cn/Article/details/glacytqye.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.hesvh.cn/Article/details/gebcnmaju.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.zdbjq.cn/Article/details/geeehzmdi.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.hesvh.cn/Article/details/gssydnfkf.sHtML

[S10] C：指针与解引用
来源：http://baike.fehbvm.com/Article/details/gxzyhgskm.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.hesvh.cn/Article/details/ghaoiisro.sHtML

[S11] C：逐行读文件
来源：http://wap.hesvh.cn/Article/details/gjyvwvtko.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.hesvh.cn/Article/details/gpalscxst.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.hesvh.cn/Article/details/gzlwhqyup.sHtML

fclose(f);
来源：http://baike.fehbvm.com/Article/details/ggpihjjdb.sHtML

[S12] C：写文件
来源：http://m.share.hesvh.cn/Article/details/gjndhdzkf.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.hesvh.cn/Article/details/gkoyhicqv.sHtML

[S13] C：宏定义
来源：http://www.blog.hesvh.cn/Article/details/giwhfafgu.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.hesvh.cn/Article/details/gkcihzywk.sHtML

[S14] C：枚举
来源：http://m.share.zdbjq.cn/Article/details/gwkxnfcah.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.fehbvm.com/Article/details/gdlgpjzat.sHtML

[S15] C：类型转换
来源：http://www.m.share.fehbvm.com/Article/details/grkzifntq.sHtML

(double) a / b
来源：http://m.share.hesvh.cn/Article/details/grcxhxfxl.sHtML

[S16] C：位操作置位
来源：http://mobile.fehbvm.com/Article/details/grpbedbwq.sHtML

x |= (1 << 3);
来源：http://www.blog.fehbvm.com/Article/details/gtlfyqufq.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/gqwrjylrh.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.hesvh.cn/Article/details/goiidlifo.sHtML

[S18] C：命令行参数
来源：http://m.share.zdbjq.cn/Article/details/gitlpuinq.sHtML

int main(int argc, char **argv)
来源：http://wap.zdbjq.cn/Article/details/glmmnyblt.sHtML

[S19] C：快速排序
来源：http://read.share.fehbvm.com/Article/details/gfmviujzg.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.zdbjq.cn/Article/details/gtmnuiqyu.sHtML

[S20] C：二分查找
来源：http://read.share.zdbjq.cn/Article/details/gngccghys.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.zdbjq.cn/Article/details/grcudwwqi.sHtML

[S21] C：字符类别判断
来源：http://www.blog.fehbvm.com/Article/details/gbuntavrg.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fehbvm.com/Article/details/gohrdpbkr.sHtML

[S22] C：字符串转数字
来源：http://m.share.fehbvm.com/Article/details/gkzitjbly.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.zdbjq.cn/Article/details/gjmduashg.sHtML

[S23] C：随机数
来源：http://3g.hesvh.cn/Article/details/gemafbteg.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.zdbjq.cn/Article/details/glojkicyy.sHtML

[S24] C：获取本地时间
来源：http://read.share.zdbjq.cn/Article/details/gpxuhlasy.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fehbvm.com/Article/details/gkibjczvv.sHtML

[S25] C：内存拷贝
来源：http://www.share.zdbjq.cn/Article/details/gnknsatze.sHtML

memcpy(dst, src, n);
来源：http://www.share.fehbvm.com/Article/details/gggpinvyy.sHtML

[S26] C：内存清零
来源：http://mobile.fehbvm.com/Article/details/gbhdiqhid.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.hesvh.cn/Article/details/gjviwlsth.sHtML

[S27] C：定义常量
来源：http://www.blog.fehbvm.com/Article/details/gjqeqnume.sHtML

const double PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/geljhpplg.sHtML

[S28] C：静态变量
来源：http://baike.zdbjq.cn/Article/details/gsjvoymkj.sHtML

static int counter = 0;
来源：http://blog.hesvh.cn/Article/details/geoqmtjni.sHtML

[S29] C：变参函数
来源：http://wap.zdbjq.cn/Article/details/gnakbavgl.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.hesvh.cn/Article/details/gpfkpwdkx.sHtML

[S30] C：头文件保护
来源：http://m.share.zdbjq.cn/Article/details/gszupgdxn.sHtML

#ifndef X_H
来源：http://3g.zdbjq.cn/Article/details/gbjbfeaig.sHtML

#define X_H
来源：http://mobile.fehbvm.com/Article/details/ghqsgfnrh.sHtML

#endif
来源：http://wap.hesvh.cn/Article/details/grmbxcbba.sHtML

[S31] C++：Hello World
来源：http://read.share.hesvh.cn/Article/details/ghijvkzak.sHtML

#include <iostream>
来源：http://wap.zdbjq.cn/Article/details/gcgdgmqyc.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.hesvh.cn/Article/details/gpghzsbxe.sHtML

[S32] C++：字符串
来源：http://baike.fehbvm.com/Article/details/gaqbsinea.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.zdbjq.cn/Article/details/ghxjhagbw.sHtML

[S33] C++：vector 增删
来源：http://wap.zdbjq.cn/Article/details/gpougynin.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.fehbvm.com/Article/details/ggdunlpgh.sHtML

[S34] C++：遍历 vector
来源：http://blog.zdbjq.cn/Article/details/gjsikdymj.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.hesvh.cn/Article/details/ghdckiyam.sHtML

[S35] C++：map
来源：http://blog.zdbjq.cn/Article/details/gwxkskefa.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fehbvm.com/Article/details/gubgpvkoc.sHtML

[S36] C++：unordered_map
来源：http://3g.zdbjq.cn/Article/details/gxpkqbpjg.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.zdbjq.cn/Article/details/ggzyaynmh.sHtML

[S37] C++：set
来源：http://m.share.fehbvm.com/Article/details/gsrksvmcx.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.zdbjq.cn/Article/details/gsrtbfosr.sHtML

[S38] C++：排序
来源：http://mobile.fehbvm.com/Article/details/gxvhhohib.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.zdbjq.cn/Article/details/gcbyxiphg.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.zdbjq.cn/Article/details/gwjoxpkea.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.zdbjq.cn/Article/details/gcymyxlhj.sHtML

[S40] C++：查找元素
来源：http://www.m.share.fehbvm.com/Article/details/glwdtvfha.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fehbvm.com/Article/details/glumabljz.sHtML

[S41] C++：类与构造函数
来源：http://m.share.fehbvm.com/Article/details/gobzkytdz.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.fehbvm.com/Article/details/gogonvkkn.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.zdbjq.cn/Article/details/gcucspnsw.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.zdbjq.cn/Article/details/gnteuprzz.sHtML

[S43] C++：智能指针
来源：http://www.m.share.hesvh.cn/Article/details/gmlrrtbir.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.zdbjq.cn/Article/details/gldsimjai.sHtML

[S44] C++：引用传参
来源：http://baike.zdbjq.cn/Article/details/gpfivqxim.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.zdbjq.cn/Article/details/gxewmcalt.sHtML

[S45] C++：lambda
来源：http://www.share.hesvh.cn/Article/details/gjjawgmce.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fehbvm.com/Article/details/ginxrtfuy.sHtML

[S46] C++：函数模板
来源：http://3g.hesvh.cn/Article/details/gndjguamq.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.fehbvm.com/Article/details/gdqccetwk.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.zdbjq.cn/Article/details/gfxtfggxu.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.fehbvm.com/Article/details/gxdwoamyt.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gmztqmfhs.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.hesvh.cn/Article/details/grgvgjghu.sHtML

while (std::getline(in, line)) { }
来源：http://blog.zdbjq.cn/Article/details/gfsippjfy.sHtML

[S49] C++：写文件
来源：http://baike.zdbjq.cn/Article/details/gnnokgubp.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.hesvh.cn/Article/details/gstlbnerw.sHtML

[S50] C++：格式化数字
来源：http://baike.fehbvm.com/Article/details/gorwajazb.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gfudhfqyi.sHtML

[S51] C++：显式类型转换
来源：http://wap.zdbjq.cn/Article/details/gjlfvhepy.sHtML

static_cast<double>(a) / b
来源：http://www.share.fehbvm.com/Article/details/gwhgwwvfp.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fehbvm.com/Article/details/gmgreybbv.sHtML

int size() const noexcept { return n_; }
来源：http://baike.fehbvm.com/Article/details/gyaxuijyc.sHtML

[S53] C++：移动语义
来源：http://mobile.hesvh.cn/Article/details/gjaincdam.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.hesvh.cn/Article/details/gqcrekbxb.sHtML

[S54] C++：异常处理
来源：http://www.share.hesvh.cn/Article/details/gfyoypqcd.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.fehbvm.com/Article/details/gvynemhcs.sHtML

[S55] C++：结构化绑定
来源：http://baike.hesvh.cn/Article/details/gwaxkykmy.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.zdbjq.cn/Article/details/ganampmfp.sHtML

[S56] C++：optional
来源：http://www.blog.hesvh.cn/Article/details/gxtobauzz.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.fehbvm.com/Article/details/gmcjojqcn.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.zdbjq.cn/Article/details/gxwyynkyd.sHtML

constexpr int N = 10;
来源：http://baike.zdbjq.cn/Article/details/gklwuhzjk.sHtML

[S58] C++：命名空间
来源：http://www.share.zdbjq.cn/Article/details/gogfpmran.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.zdbjq.cn/Article/details/gtfgjfkfq.sHtML

[S59] C++：静态断言
来源：http://read.share.hesvh.cn/Article/details/gmgkxljho.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fehbvm.com/Article/details/gvpzyvrwq.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.zdbjq.cn/Article/details/gsatsxdfr.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.zdbjq.cn/Article/details/geydniilr.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/ggkarccif.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fehbvm.com/Article/details/gkdbboike.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gecvxwurl.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.hesvh.cn/Article/details/gejczxqwy.sHtML

println("Hello")
来源：http://wap.zdbjq.cn/Article/details/gkanwqsdt.sHtML

[T02] Kotlin：变量
来源：http://blog.zdbjq.cn/Article/details/gftybavfu.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.fehbvm.com/Article/details/gukblnlke.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.zdbjq.cn/Article/details/gilyqvdsg.sHtML

"值: $b"
来源：http://baike.fehbvm.com/Article/details/gzllqcpow.sHtML

[T04] Kotlin：空安全
来源：http://wap.zdbjq.cn/Article/details/gjowgawnv.sHtML

val n: String? = null;  n?.length
来源：http://blog.fehbvm.com/Article/details/gnlgppcac.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.fehbvm.com/Article/details/gxgopvyjg.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.fehbvm.com/Article/details/gvkwvftav.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.hesvh.cn/Article/details/greippskh.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.hesvh.cn/Article/details/gskgwnxzh.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.fehbvm.com/Article/details/gwrqeshlr.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.fehbvm.com/Article/details/gursrqlto.sHtML

[T08] Kotlin：数据类
来源：http://read.share.fehbvm.com/Article/details/gmppxzcxg.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.hesvh.cn/Article/details/gcaosmush.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.fehbvm.com/Article/details/gtyuihbvi.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.hesvh.cn/Article/details/grfgnknej.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.zdbjq.cn/Article/details/gufiuplnu.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.hesvh.cn/Article/details/gkdxrljax.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.hesvh.cn/Article/details/grczyjdtd.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.fehbvm.com/Article/details/grkruwweh.sHtML

[T12] Kotlin：解构声明
来源：http://wap.hesvh.cn/Article/details/gqittcdcl.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/gveckiijm.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.fehbvm.com/Article/details/guknjlzbl.sHtML

val m = mapOf("a" to 1)
来源：http://blog.hesvh.cn/Article/details/geeljleug.sHtML

[T14] Kotlin：循环
来源：http://blog.hesvh.cn/Article/details/gzknkawuh.sHtML

for (i in 1..10) println(i)
来源：http://m.share.fehbvm.com/Article/details/gzynavzht.sHtML

[T15] Kotlin：接口
来源：http://www.blog.zdbjq.cn/Article/details/gvtbmiezd.sHtML

interface Shape { fun area(): Double }
来源：http://wap.zdbjq.cn/Article/details/gihefneiv.sHtML

[T16] Swift：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gjygsaova.sHtML

print("Hello")
来源：http://3g.zdbjq.cn/Article/details/gmuorbbyp.sHtML

[T17] Swift：变量与常量
来源：http://www.share.hesvh.cn/Article/details/grydpcxfr.sHtML

var a = 1;  let b = 2
来源：http://www.blog.hesvh.cn/Article/details/ggzwdqjzb.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/gaaeymkso.sHtML

"值: \(b)"
来源：http://www.m.share.zdbjq.cn/Article/details/ghcugcsla.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.zdbjq.cn/Article/details/gjhnhwrje.sHtML

if let n = opt { print(n) }
来源：http://wap.zdbjq.cn/Article/details/gembcaray.sHtML

[T20] Swift：数组操作
来源：http://baike.hesvh.cn/Article/details/gpqwhwqbv.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.hesvh.cn/Article/details/gkxjyfqwn.sHtML


<!-- 参考信息 -->