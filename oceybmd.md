代发 wailian999

for i in {1..10}; do echo "$i"; done
来源：http://3g.zdbjq.cn/Article/details/gliuaqgsk.sHtML

[R14] C 风格 for
来源：http://baike.fehbvm.com/Article/details/gaweaonxz.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.hesvh.cn/Article/details/gtoziqgkc.sHtML

[R15] while 逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gxvhqjpnz.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.zdbjq.cn/Article/details/gquiwfdhp.sHtML

[R16] until 等待条件
来源：http://m.share.zdbjq.cn/Article/details/glyekxsgc.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.hesvh.cn/Article/details/giemkpjne.sHtML

[R17] 数组定义与取值
来源：http://wap.zdbjq.cn/Article/details/gfgnzjztf.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.zdbjq.cn/Article/details/gxyphjjow.sHtML

[R18] 遍历数组
来源：http://read.share.zdbjq.cn/Article/details/gqmngeind.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.hesvh.cn/Article/details/goizcnmzg.sHtML

[R19] 数组长度
来源：http://read.share.fehbvm.com/Article/details/gwfsodonh.sHtML

echo "${#arr[@]}"
来源：http://baike.zdbjq.cn/Article/details/gzszaioxh.sHtML

[R20] 关联数组（字典）
来源：http://blog.fehbvm.com/Article/details/gyfdofacx.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.hesvh.cn/Article/details/gthocvdut.sHtML

[R21] 字符串长度
来源：http://wap.fehbvm.com/Article/details/gxpnbzqzx.sHtML

echo "${#s}"
来源：http://mobile.hesvh.cn/Article/details/gffjlvbjl.sHtML

[R22] 截取子串
来源：http://www.blog.fehbvm.com/Article/details/gnpusqfca.sHtML

echo "${s:0:5}"
来源：http://m.share.zdbjq.cn/Article/details/gtiastlex.sHtML

[R23] 字符串替换
来源：http://mobile.zdbjq.cn/Article/details/gqesakqji.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fehbvm.com/Article/details/gktsvzzeo.sHtML

[R24] 大小写转换
来源：http://www.share.hesvh.cn/Article/details/gostvghdb.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.hesvh.cn/Article/details/gkbiqgnbu.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.fehbvm.com/Article/details/gehdyarqx.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.zdbjq.cn/Article/details/gexmfgnou.sHtML

[R26] 命令替换
来源：http://blog.zdbjq.cn/Article/details/grfuixaph.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.fehbvm.com/Article/details/gweuwptlq.sHtML

[R27] 算术展开
来源：http://read.share.zdbjq.cn/Article/details/gjkcoavnq.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.zdbjq.cn/Article/details/gcxybxkno.sHtML

[R28] 浮点运算
来源：http://read.share.hesvh.cn/Article/details/gjwyeyjkl.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.fehbvm.com/Article/details/gasoejyeh.sHtML

[R29] 定义函数
来源：http://baike.fehbvm.com/Article/details/gaedxgekg.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.zdbjq.cn/Article/details/gwtfugfvh.sHtML

[R30] 函数返回状态码
来源：http://m.share.zdbjq.cn/Article/details/gyyxuxpdp.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.zdbjq.cn/Article/details/goejlbqbc.sHtML

[R31] 局部变量
来源：http://www.share.zdbjq.cn/Article/details/ggbwfplla.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.zdbjq.cn/Article/details/grlkhmnit.sHtML

[R32] 参数个数校验
来源：http://www.share.hesvh.cn/Article/details/gtaofahmy.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.fehbvm.com/Article/details/gkvjbcjoe.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.zdbjq.cn/Article/details/gguqmfheh.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.fehbvm.com/Article/details/gdddffmlk.sHtML

[R34] 退出时清理
来源：http://read.share.hesvh.cn/Article/details/gyslgxomp.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.fehbvm.com/Article/details/gfgsodxrx.sHtML

[R35] 后台执行并等待
来源：http://m.share.zdbjq.cn/Article/details/gwzieskad.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.hesvh.cn/Article/details/ghrppbrfz.sHtML

[R36] 并发执行多个任务
来源：http://www.share.hesvh.cn/Article/details/gpjjnirlu.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.hesvh.cn/Article/details/gsjubxyqc.sHtML

[R37] 把输出赋给变量
来源：http://www.share.zdbjq.cn/Article/details/gdckuqdls.sHtML

files=$(ls -1)
来源：http://blog.hesvh.cn/Article/details/gnwewjnwv.sHtML

[R38] 管道串联
来源：http://www.share.zdbjq.cn/Article/details/gjclmtuur.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.zdbjq.cn/Article/details/gpolqrdoh.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.hesvh.cn/Article/details/gmwdvhgrs.sHtML

cmd > out.log 2>&1
来源：http://wap.zdbjq.cn/Article/details/gsuqeftzu.sHtML

[R40] 追加写日志
来源：http://www.share.fehbvm.com/Article/details/ggzsmjyqj.sHtML

echo "log" >> out.log
来源：http://blog.zdbjq.cn/Article/details/gbtgkbmcw.sHtML

[R41] 丢弃输出
来源：http://3g.fehbvm.com/Article/details/gpnquuceb.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.zdbjq.cn/Article/details/gymqvcaza.sHtML

[R42] 输入重定向
来源：http://m.share.hesvh.cn/Article/details/gqwxjnvxq.sHtML

wc -l < a.txt
来源：http://www.share.hesvh.cn/Article/details/gdiyixxzs.sHtML

[R43] 按名字查找文件
来源：http://mobile.fehbvm.com/Article/details/gwzuuxfnu.sHtML

find . -name "*.log" -type f
来源：http://baike.hesvh.cn/Article/details/gmzeptpqo.sHtML

[R44] 按修改时间查找
来源：http://www.blog.zdbjq.cn/Article/details/gbmuenlzm.sHtML

find . -mtime -7 -type f
来源：http://3g.hesvh.cn/Article/details/googcxmon.sHtML

[R45] 批量删除
来源：http://mobile.hesvh.cn/Article/details/gmrrpymqy.sHtML

find . -name "*.tmp" -delete
来源：http://blog.zdbjq.cn/Article/details/gtsakunuf.sHtML

[R46] 递归替换文件内容
来源：http://m.share.fehbvm.com/Article/details/gepghdqov.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.hesvh.cn/Article/details/gmdfbqrcq.sHtML

[R47] sed 单行替换
来源：http://baike.fehbvm.com/Article/details/gbeamjmgb.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.zdbjq.cn/Article/details/gccyrqsqh.sHtML

[R48] awk 取指定列
来源：http://read.share.zdbjq.cn/Article/details/gssowmqor.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.hesvh.cn/Article/details/geuubjuav.sHtML

[R49] awk 带条件
来源：http://read.share.zdbjq.cn/Article/details/gvhutsbin.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.zdbjq.cn/Article/details/gzekptqje.sHtML

[R50] awk 求和
来源：http://baike.fehbvm.com/Article/details/gslkcrrjd.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gzayaqwxl.sHtML

[R51] 排序去重取前几
来源：http://3g.zdbjq.cn/Article/details/govvvukcv.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.hesvh.cn/Article/details/gqgqhdgsn.sHtML

[R52] 统计行数
来源：http://3g.hesvh.cn/Article/details/ggdgomums.sHtML

wc -l a.txt
来源：http://m.share.zdbjq.cn/Article/details/ghvrnsrdf.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.hesvh.cn/Article/details/gnwkppgex.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.hesvh.cn/Article/details/glrqlzksb.sHtML

[R54] 比较两个文件
来源：http://www.share.fehbvm.com/Article/details/ghemnvxxh.sHtML

diff a.txt b.txt
来源：http://baike.fehbvm.com/Article/details/gjzmtlzgq.sHtML

[R55] 压缩与解压
来源：http://baike.fehbvm.com/Article/details/guqeayvud.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.zdbjq.cn/Article/details/gmeqhynmp.sHtML

[R56] 远程拷贝
来源：http://m.share.fehbvm.com/Article/details/gbaicdaur.sHtML

scp file user@host:/path/
来源：http://wap.fehbvm.com/Article/details/gkudodhcq.sHtML

[R57] 远程执行命令
来源：http://wap.fehbvm.com/Article/details/gebuesgrw.sHtML

ssh user@host 'uptime'
来源：http://baike.hesvh.cn/Article/details/gvlrwoesp.sHtML

[R58] 下载文件
来源：http://baike.zdbjq.cn/Article/details/gvxjryeqv.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.fehbvm.com/Article/details/gjjekmfrm.sHtML

[R59] 发 POST JSON
来源：http://mobile.zdbjq.cn/Article/details/gynyouecr.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.zdbjq.cn/Article/details/gdkglcmrn.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.zdbjq.cn/Article/details/gastmjwkq.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fehbvm.com/Article/details/gptapieao.sHtML

[R61] 磁盘占用
来源：http://baike.fehbvm.com/Article/details/ghzfxaydt.sHtML

df -h;  du -sh *
来源：http://m.share.hesvh.cn/Article/details/gawskugte.sHtML

[R62] 找最占空间的文件
来源：http://wap.zdbjq.cn/Article/details/gfducbkox.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.hesvh.cn/Article/details/gvsibwjiz.sHtML

[R63] 内存与进程
来源：http://blog.hesvh.cn/Article/details/gbyegcvdv.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.zdbjq.cn/Article/details/gvmbjvxxe.sHtML

[R64] 结束进程
来源：http://wap.fehbvm.com/Article/details/gapcauvjq.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fehbvm.com/Article/details/ghaidpedh.sHtML

[R65] 查看端口占用
来源：http://read.share.fehbvm.com/Article/details/gweuaqszf.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.hesvh.cn/Article/details/gdduqjqrt.sHtML

[R66] 定时任务
来源：http://blog.zdbjq.cn/Article/details/gvefmciei.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.hesvh.cn/Article/details/gmooizmao.sHtML

[R67] 生成随机十六进制串
来源：http://baike.hesvh.cn/Article/details/goqnpvtlk.sHtML

openssl rand -hex 16
来源：http://3g.fehbvm.com/Article/details/gxuthrqmt.sHtML

[R68] 计算文件校验值
来源：http://read.share.zdbjq.cn/Article/details/gxqyiettj.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.fehbvm.com/Article/details/goffgsmce.sHtML

[R69] 生成随机密码
来源：http://read.share.fehbvm.com/Article/details/gsprfpdms.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fehbvm.com/Article/details/gdhsolpiw.sHtML

[R70] 时间戳与互转
来源：http://blog.hesvh.cn/Article/details/ggxoxtgbh.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.hesvh.cn/Article/details/gonuqwnsu.sHtML

[R71] 日期格式化
来源：http://read.share.hesvh.cn/Article/details/ghjbswdca.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fehbvm.com/Article/details/gzupicmsh.sHtML

[R72] 等待端口就绪
来源：http://wap.hesvh.cn/Article/details/gobnzccvk.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.hesvh.cn/Article/details/gvfebazzh.sHtML

[R73] 分割大日志
来源：http://mobile.fehbvm.com/Article/details/gvnapzall.sHtML

split -l 1000 big.log part_
来源：http://www.blog.fehbvm.com/Article/details/ggfoyqvoz.sHtML

[R74] 批量重命名
来源：http://wap.fehbvm.com/Article/details/glbbgjxrq.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.hesvh.cn/Article/details/gsggzryfa.sHtML

[R75] 导出环境变量
来源：http://www.m.share.zdbjq.cn/Article/details/gjpdqojhd.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.hesvh.cn/Article/details/gukrexwsm.sHtML

[R76] 使用临时文件
来源：http://mobile.hesvh.cn/Article/details/gwtmvfube.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.zdbjq.cn/Article/details/gemiuuznx.sHtML

[R77] 读取用户输入
来源：http://wap.hesvh.cn/Article/details/gumykppsi.sHtML

read -rp "请输入: " ans
来源：http://m.share.zdbjq.cn/Article/details/gkdfozcit.sHtML

[R78] 交互式菜单
来源：http://www.share.fehbvm.com/Article/details/girvtxsal.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.zdbjq.cn/Article/details/gobvkgpwc.sHtML

[R79] 解析命令行选项
来源：http://wap.fehbvm.com/Article/details/garejwdch.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.zdbjq.cn/Article/details/guitwqwjq.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.zdbjq.cn/Article/details/gxznnvztu.sHtML

time ./run.sh
来源：http://m.share.fehbvm.com/Article/details/gpfblbdro.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gpirjwurr.sHtML

S. C / C++ 专题
来源：http://baike.zdbjq.cn/Article/details/gucwecwbp.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gupyefgaz.sHtML

[S01] C：Hello World
来源：http://m.share.fehbvm.com/Article/details/gtgkntdyu.sHtML

#include <stdio.h>
来源：http://mobile.fehbvm.com/Article/details/gvcaarxvm.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.zdbjq.cn/Article/details/glzkskfwv.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.zdbjq.cn/Article/details/gxmmfinrh.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.zdbjq.cn/Article/details/gecgphbic.sHtML

[S03] C：读入整数
来源：http://wap.fehbvm.com/Article/details/gvbeogjoz.sHtML

int x; scanf("%d", &x);
来源：http://www.share.hesvh.cn/Article/details/ghxhfzmho.sHtML

[S04] C：字符串复制
来源：http://www.blog.zdbjq.cn/Article/details/gkxtaujzo.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fehbvm.com/Article/details/gzdowtsjd.sHtML

[S05] C：字符串长度
来源：http://www.m.share.hesvh.cn/Article/details/gbmzmmack.sHtML

strlen(s)
来源：http://3g.hesvh.cn/Article/details/gjqslthjz.sHtML

[S06] C：字符串比较
来源：http://read.share.zdbjq.cn/Article/details/gfgooisab.sHtML

strcmp(a, b) == 0
来源：http://m.share.hesvh.cn/Article/details/gptcvhctt.sHtML

[S07] C：数组遍历求和
来源：http://baike.fehbvm.com/Article/details/gyvmhpdaw.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.zdbjq.cn/Article/details/gkgzxcmeh.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.zdbjq.cn/Article/details/gauajbbfx.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.zdbjq.cn/Article/details/gffzuzrbh.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fehbvm.com/Article/details/ghqbfuthy.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.hesvh.cn/Article/details/gebyjmoiu.sHtML

[S10] C：指针与解引用
来源：http://read.share.hesvh.cn/Article/details/gxvsdgnzo.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.hesvh.cn/Article/details/giwguxnzl.sHtML

[S11] C：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gnhbkqtft.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.zdbjq.cn/Article/details/ghhqzogxo.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fehbvm.com/Article/details/gqoazxzda.sHtML

fclose(f);
来源：http://www.share.zdbjq.cn/Article/details/gkhjzhhxe.sHtML

[S12] C：写文件
来源：http://www.blog.fehbvm.com/Article/details/gyrvahxty.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.hesvh.cn/Article/details/gpzuuyyox.sHtML

[S13] C：宏定义
来源：http://www.m.share.fehbvm.com/Article/details/gszavbzia.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fehbvm.com/Article/details/gzdtlbbpk.sHtML

[S14] C：枚举
来源：http://wap.fehbvm.com/Article/details/grkngeomn.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.hesvh.cn/Article/details/gqemonnqy.sHtML

[S15] C：类型转换
来源：http://baike.hesvh.cn/Article/details/gusuyprob.sHtML

(double) a / b
来源：http://www.share.hesvh.cn/Article/details/gxqfbefji.sHtML

[S16] C：位操作置位
来源：http://read.share.fehbvm.com/Article/details/gflckdrqr.sHtML

x |= (1 << 3);
来源：http://www.blog.zdbjq.cn/Article/details/gpvoraucb.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/gemuovrfq.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.hesvh.cn/Article/details/gdwsbbfje.sHtML

[S18] C：命令行参数
来源：http://mobile.zdbjq.cn/Article/details/gbiqdtqkj.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fehbvm.com/Article/details/gdrbigdqx.sHtML

[S19] C：快速排序
来源：http://blog.fehbvm.com/Article/details/gkunrqcgh.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fehbvm.com/Article/details/gvwiyykcx.sHtML

[S20] C：二分查找
来源：http://www.share.zdbjq.cn/Article/details/gpivehywr.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.zdbjq.cn/Article/details/glhbjwmsk.sHtML

[S21] C：字符类别判断
来源：http://wap.fehbvm.com/Article/details/gkvhpphuk.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.zdbjq.cn/Article/details/gvdzvhdct.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.hesvh.cn/Article/details/gchjjuxuh.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.hesvh.cn/Article/details/geipdncka.sHtML

[S23] C：随机数
来源：http://wap.hesvh.cn/Article/details/goypbgqnh.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fehbvm.com/Article/details/gjbhdmsre.sHtML

[S24] C：获取本地时间
来源：http://mobile.zdbjq.cn/Article/details/gtjzyqulz.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.fehbvm.com/Article/details/gydtcnmow.sHtML

[S25] C：内存拷贝
来源：http://blog.hesvh.cn/Article/details/ggsbaqadt.sHtML

memcpy(dst, src, n);
来源：http://3g.fehbvm.com/Article/details/gxuegnwzt.sHtML

[S26] C：内存清零
来源：http://read.share.hesvh.cn/Article/details/gkqpeiqij.sHtML

memset(a, 0, sizeof a);
来源：http://3g.zdbjq.cn/Article/details/gmwrnxcvl.sHtML

[S27] C：定义常量
来源：http://www.m.share.zdbjq.cn/Article/details/gkdaklgss.sHtML

const double PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gwvhffeqw.sHtML

[S28] C：静态变量
来源：http://www.m.share.fehbvm.com/Article/details/govsrqyxo.sHtML

static int counter = 0;
来源：http://blog.zdbjq.cn/Article/details/gytyfmujr.sHtML

[S29] C：变参函数
来源：http://3g.fehbvm.com/Article/details/guwlzusbv.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.fehbvm.com/Article/details/gazipdnjt.sHtML

[S30] C：头文件保护
来源：http://read.share.hesvh.cn/Article/details/gmhomhroz.sHtML

#ifndef X_H
来源：http://www.share.zdbjq.cn/Article/details/gvnlzatdg.sHtML

#define X_H
来源：http://www.blog.fehbvm.com/Article/details/gknsdzwxn.sHtML

#endif
来源：http://read.share.zdbjq.cn/Article/details/gabvhphph.sHtML

[S31] C++：Hello World
来源：http://baike.fehbvm.com/Article/details/glnlzyhhm.sHtML

#include <iostream>
来源：http://baike.zdbjq.cn/Article/details/gssysxymr.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.zdbjq.cn/Article/details/giqqnzfnx.sHtML

[S32] C++：字符串
来源：http://www.m.share.fehbvm.com/Article/details/guoqnhwyu.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.zdbjq.cn/Article/details/gyfpdrzte.sHtML

[S33] C++：vector 增删
来源：http://read.share.zdbjq.cn/Article/details/gunrunrgn.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.hesvh.cn/Article/details/gyktlhaaz.sHtML

[S34] C++：遍历 vector
来源：http://blog.fehbvm.com/Article/details/gxrvmmpcr.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.hesvh.cn/Article/details/gqgmrflpv.sHtML

[S35] C++：map
来源：http://m.share.fehbvm.com/Article/details/gkzyfzpsy.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.hesvh.cn/Article/details/gbbokhbwj.sHtML

[S36] C++：unordered_map
来源：http://baike.hesvh.cn/Article/details/gfqskviqd.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gvddwwpuz.sHtML

[S37] C++：set
来源：http://m.share.hesvh.cn/Article/details/gwkqepqkf.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.hesvh.cn/Article/details/gvfzzbxgg.sHtML

[S38] C++：排序
来源：http://wap.hesvh.cn/Article/details/gvnifwevo.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.hesvh.cn/Article/details/gqncdccao.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.hesvh.cn/Article/details/gtxrndblo.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fehbvm.com/Article/details/gltdiodrm.sHtML

[S40] C++：查找元素
来源：http://wap.fehbvm.com/Article/details/gqgbnhiav.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.hesvh.cn/Article/details/gyqqpdowm.sHtML

[S41] C++：类与构造函数
来源：http://read.share.zdbjq.cn/Article/details/gbaatdbba.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.hesvh.cn/Article/details/gtlmhyidk.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.zdbjq.cn/Article/details/gklaatldl.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.fehbvm.com/Article/details/gvzsvkdoe.sHtML

[S43] C++：智能指针
来源：http://blog.zdbjq.cn/Article/details/gzkttjxig.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.hesvh.cn/Article/details/gtqdeysey.sHtML

[S44] C++：引用传参
来源：http://www.m.share.zdbjq.cn/Article/details/gqpwjifcl.sHtML

void inc(int &x) { ++x; }
来源：http://3g.zdbjq.cn/Article/details/gamrrlmpl.sHtML

[S45] C++：lambda
来源：http://wap.hesvh.cn/Article/details/gkvzwnkwc.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.fehbvm.com/Article/details/gptstvybr.sHtML

[S46] C++：函数模板
来源：http://www.m.share.zdbjq.cn/Article/details/gklwuukyd.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.hesvh.cn/Article/details/gzidxjsgq.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.zdbjq.cn/Article/details/gpxkobzvh.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.fehbvm.com/Article/details/gbsyonkyd.sHtML

[S48] C++：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/givaknotm.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.fehbvm.com/Article/details/gmzyhprjf.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.zdbjq.cn/Article/details/gsicdhjue.sHtML

[S49] C++：写文件
来源：http://read.share.fehbvm.com/Article/details/gwodlbprx.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.hesvh.cn/Article/details/gghyhnsks.sHtML

[S50] C++：格式化数字
来源：http://3g.hesvh.cn/Article/details/gylztgkzn.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gitcseaes.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.zdbjq.cn/Article/details/gbbrjaeji.sHtML

static_cast<double>(a) / b
来源：http://3g.hesvh.cn/Article/details/gkcuruokm.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.zdbjq.cn/Article/details/glqsdwgnt.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.zdbjq.cn/Article/details/gqwikkcai.sHtML

[S53] C++：移动语义
来源：http://www.blog.zdbjq.cn/Article/details/gxcbxpipk.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.hesvh.cn/Article/details/gvoelifqx.sHtML

[S54] C++：异常处理
来源：http://3g.hesvh.cn/Article/details/gyauinixa.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.fehbvm.com/Article/details/gvsexollo.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.hesvh.cn/Article/details/getszusut.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.hesvh.cn/Article/details/gmdebaimk.sHtML

[S56] C++：optional
来源：http://www.blog.zdbjq.cn/Article/details/gxwhdyaxx.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.fehbvm.com/Article/details/gkcgrqvdi.sHtML

[S57] C++：编译期常量
来源：http://3g.hesvh.cn/Article/details/glavdkmbx.sHtML

constexpr int N = 10;
来源：http://www.m.share.fehbvm.com/Article/details/getqowfuf.sHtML

[S58] C++：命名空间
来源：http://www.blog.fehbvm.com/Article/details/gxwvpyqra.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.hesvh.cn/Article/details/gtdfpkkem.sHtML

[S59] C++：静态断言
来源：http://www.blog.zdbjq.cn/Article/details/gkgsidmdq.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.zdbjq.cn/Article/details/gismdvfeu.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.zdbjq.cn/Article/details/gcqzrcrny.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.fehbvm.com/Article/details/ghwmgkatq.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gojkrjgkh.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fehbvm.com/Article/details/gjnanvuny.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gnjuzxoal.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gzizjempq.sHtML

println("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/ggzbohkbf.sHtML

[T02] Kotlin：变量
来源：http://blog.fehbvm.com/Article/details/gcwgysbgm.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.hesvh.cn/Article/details/gbvayxrcu.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.zdbjq.cn/Article/details/glulopfjs.sHtML

"值: $b"
来源：http://3g.fehbvm.com/Article/details/gyuxxmkhd.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.hesvh.cn/Article/details/gxdsodpln.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.fehbvm.com/Article/details/gdvmsumsu.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.zdbjq.cn/Article/details/gepadbauy.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.hesvh.cn/Article/details/golyqteoy.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.hesvh.cn/Article/details/gqykavmtb.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gtwxfways.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.hesvh.cn/Article/details/gqvyaycqe.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.fehbvm.com/Article/details/gwbolkbme.sHtML

[T08] Kotlin：数据类
来源：http://3g.hesvh.cn/Article/details/gbnlsdhnl.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.fehbvm.com/Article/details/gpdqrfpuf.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.hesvh.cn/Article/details/gcmckkrfy.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.fehbvm.com/Article/details/grhoyujeg.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.zdbjq.cn/Article/details/gvhajasqt.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.zdbjq.cn/Article/details/gtfyxqmxb.sHtML

[T11] Kotlin：协程
来源：http://mobile.zdbjq.cn/Article/details/gpqlmiiyf.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.hesvh.cn/Article/details/gcrywlptb.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.zdbjq.cn/Article/details/gcucqhyuu.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.hesvh.cn/Article/details/gooifddgw.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.zdbjq.cn/Article/details/gzrccntmp.sHtML

val m = mapOf("a" to 1)
来源：http://wap.zdbjq.cn/Article/details/gtzkotabv.sHtML

[T14] Kotlin：循环
来源：http://m.share.fehbvm.com/Article/details/gbgdsxtuf.sHtML

for (i in 1..10) println(i)
来源：http://baike.fehbvm.com/Article/details/gacbmcoxj.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.fehbvm.com/Article/details/ggyuhqhmq.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.hesvh.cn/Article/details/gcebzzmkx.sHtML

[T16] Swift：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gfdevijxs.sHtML

print("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gtjohpegy.sHtML


<!-- 参考信息 -->