代发 wailian999

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.hesvh.cn/Article/details/gdkdpboka.sHtML

[R16] until 等待条件
来源：http://read.share.zdbjq.cn/Article/details/grshkqtgb.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.zdbjq.cn/Article/details/gxepgttlu.sHtML

[R17] 数组定义与取值
来源：http://wap.hesvh.cn/Article/details/glikrwygk.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.hesvh.cn/Article/details/gxktvoqid.sHtML

[R18] 遍历数组
来源：http://www.share.fehbvm.com/Article/details/gnvrrbbpd.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.zdbjq.cn/Article/details/gczvfadub.sHtML

[R19] 数组长度
来源：http://www.m.share.zdbjq.cn/Article/details/grjuspjxf.sHtML

echo "${#arr[@]}"
来源：http://www.blog.hesvh.cn/Article/details/gknvmhpuq.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.hesvh.cn/Article/details/gqminlvov.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.hesvh.cn/Article/details/gijyytbvf.sHtML

[R21] 字符串长度
来源：http://www.blog.fehbvm.com/Article/details/gndfjxjdq.sHtML

echo "${#s}"
来源：http://www.m.share.fehbvm.com/Article/details/gtyiagohp.sHtML

[R22] 截取子串
来源：http://www.blog.zdbjq.cn/Article/details/gbcjjpzge.sHtML

echo "${s:0:5}"
来源：http://www.m.share.fehbvm.com/Article/details/gebttpyku.sHtML

[R23] 字符串替换
来源：http://baike.fehbvm.com/Article/details/gdonajagn.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.fehbvm.com/Article/details/gwdxkodic.sHtML

[R24] 大小写转换
来源：http://www.share.fehbvm.com/Article/details/gqpcogswz.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.hesvh.cn/Article/details/gftewmmer.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.zdbjq.cn/Article/details/gtylwqruc.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.zdbjq.cn/Article/details/gxjwagfvi.sHtML

[R26] 命令替换
来源：http://www.share.zdbjq.cn/Article/details/gvsvqoluu.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.hesvh.cn/Article/details/gafncfith.sHtML

[R27] 算术展开
来源：http://baike.fehbvm.com/Article/details/gyahidadi.sHtML

echo $((1 + 2 * 3))
来源：http://wap.fehbvm.com/Article/details/ghwcqsjnc.sHtML

[R28] 浮点运算
来源：http://blog.hesvh.cn/Article/details/gtdwzizoh.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.fehbvm.com/Article/details/glikzvitc.sHtML

[R29] 定义函数
来源：http://www.blog.zdbjq.cn/Article/details/gldjminjx.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.fehbvm.com/Article/details/ghdjbkuoa.sHtML

[R30] 函数返回状态码
来源：http://mobile.hesvh.cn/Article/details/gwhpobouy.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.zdbjq.cn/Article/details/giegjhbgx.sHtML

[R31] 局部变量
来源：http://www.share.zdbjq.cn/Article/details/glgsoseib.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.hesvh.cn/Article/details/gphdnnigx.sHtML

[R32] 参数个数校验
来源：http://www.m.share.hesvh.cn/Article/details/gldujipce.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.hesvh.cn/Article/details/gjzrkvoya.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.hesvh.cn/Article/details/gsrzmsfgx.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.zdbjq.cn/Article/details/gqfbtbyrn.sHtML

[R34] 退出时清理
来源：http://read.share.fehbvm.com/Article/details/gyylfhfef.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.fehbvm.com/Article/details/gcmsracec.sHtML

[R35] 后台执行并等待
来源：http://3g.fehbvm.com/Article/details/gbblvcizn.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.fehbvm.com/Article/details/gknkawvwq.sHtML

[R36] 并发执行多个任务
来源：http://m.share.zdbjq.cn/Article/details/gurrlrxmf.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.hesvh.cn/Article/details/gsbtqsskn.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fehbvm.com/Article/details/gvgsajegp.sHtML

files=$(ls -1)
来源：http://www.blog.fehbvm.com/Article/details/gpfttwrqb.sHtML

[R38] 管道串联
来源：http://read.share.hesvh.cn/Article/details/gvtgbfjwo.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fehbvm.com/Article/details/gdnhyfycn.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.zdbjq.cn/Article/details/giwsjbzuk.sHtML

cmd > out.log 2>&1
来源：http://wap.zdbjq.cn/Article/details/gyunfyghd.sHtML

[R40] 追加写日志
来源：http://blog.zdbjq.cn/Article/details/gaazpjvtp.sHtML

echo "log" >> out.log
来源：http://www.m.share.hesvh.cn/Article/details/gycxcydly.sHtML

[R41] 丢弃输出
来源：http://www.blog.zdbjq.cn/Article/details/glbtitulx.sHtML

cmd >/dev/null 2>&1
来源：http://baike.zdbjq.cn/Article/details/ggjmhicdy.sHtML

[R42] 输入重定向
来源：http://baike.fehbvm.com/Article/details/gwbhxotdr.sHtML

wc -l < a.txt
来源：http://www.blog.fehbvm.com/Article/details/gulnnnwyh.sHtML

[R43] 按名字查找文件
来源：http://m.share.fehbvm.com/Article/details/gxjktgnla.sHtML

find . -name "*.log" -type f
来源：http://www.blog.hesvh.cn/Article/details/gtuhwbkrl.sHtML

[R44] 按修改时间查找
来源：http://baike.fehbvm.com/Article/details/gdvnqspul.sHtML

find . -mtime -7 -type f
来源：http://wap.fehbvm.com/Article/details/geadgqbwx.sHtML

[R45] 批量删除
来源：http://read.share.hesvh.cn/Article/details/gnpslmpme.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.fehbvm.com/Article/details/gskffeyxl.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.fehbvm.com/Article/details/gkcqcukmh.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fehbvm.com/Article/details/gezgcscdo.sHtML

[R47] sed 单行替换
来源：http://blog.zdbjq.cn/Article/details/gplzchbvy.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.fehbvm.com/Article/details/gmthwqcci.sHtML

[R48] awk 取指定列
来源：http://www.share.zdbjq.cn/Article/details/gzduvndim.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.fehbvm.com/Article/details/gnietbusg.sHtML

[R49] awk 带条件
来源：http://www.share.hesvh.cn/Article/details/gouufcsrh.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.zdbjq.cn/Article/details/gtxbmdtss.sHtML

[R50] awk 求和
来源：http://mobile.zdbjq.cn/Article/details/ghlaemxtv.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.hesvh.cn/Article/details/gqpapwjsk.sHtML

[R51] 排序去重取前几
来源：http://baike.hesvh.cn/Article/details/gyxbtzxmu.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.zdbjq.cn/Article/details/giozryyqu.sHtML

[R52] 统计行数
来源：http://baike.fehbvm.com/Article/details/gkqjbbkeu.sHtML

wc -l a.txt
来源：http://m.share.zdbjq.cn/Article/details/gdjptiwti.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.hesvh.cn/Article/details/gahqsbwii.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.zdbjq.cn/Article/details/gylzbxoxg.sHtML

[R54] 比较两个文件
来源：http://mobile.zdbjq.cn/Article/details/gxaqwouus.sHtML

diff a.txt b.txt
来源：http://3g.hesvh.cn/Article/details/ghsmasbwz.sHtML

[R55] 压缩与解压
来源：http://3g.fehbvm.com/Article/details/gowfghwfi.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.hesvh.cn/Article/details/gvgejeuiw.sHtML

[R56] 远程拷贝
来源：http://3g.fehbvm.com/Article/details/gxapelqzf.sHtML

scp file user@host:/path/
来源：http://wap.hesvh.cn/Article/details/gnvofpfzp.sHtML

[R57] 远程执行命令
来源：http://m.share.zdbjq.cn/Article/details/gcggdudrc.sHtML

ssh user@host 'uptime'
来源：http://read.share.hesvh.cn/Article/details/gbibqrxcp.sHtML

[R58] 下载文件
来源：http://baike.zdbjq.cn/Article/details/glnzqstvu.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.zdbjq.cn/Article/details/gojdikhuz.sHtML

[R59] 发 POST JSON
来源：http://www.share.zdbjq.cn/Article/details/gurylhwyt.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.hesvh.cn/Article/details/griykfube.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.hesvh.cn/Article/details/gfmfxozet.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.hesvh.cn/Article/details/guoboqftv.sHtML

[R61] 磁盘占用
来源：http://wap.fehbvm.com/Article/details/gfjkyauvs.sHtML

df -h;  du -sh *
来源：http://www.share.hesvh.cn/Article/details/gzdrapgpl.sHtML

[R62] 找最占空间的文件
来源：http://wap.zdbjq.cn/Article/details/gvvxpldnk.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.hesvh.cn/Article/details/gfjdgrlyc.sHtML

[R63] 内存与进程
来源：http://read.share.zdbjq.cn/Article/details/gorwchoio.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.hesvh.cn/Article/details/gmvunkkzm.sHtML

[R64] 结束进程
来源：http://3g.fehbvm.com/Article/details/gzqvsrzrg.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.hesvh.cn/Article/details/gydgfhljo.sHtML

[R65] 查看端口占用
来源：http://3g.hesvh.cn/Article/details/gfmafbahy.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.hesvh.cn/Article/details/ghzwjegie.sHtML

[R66] 定时任务
来源：http://mobile.fehbvm.com/Article/details/gktpnmkfp.sHtML

crontab -e;  crontab -l
来源：http://baike.hesvh.cn/Article/details/gtxoiixwg.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.hesvh.cn/Article/details/gapxvidyy.sHtML

openssl rand -hex 16
来源：http://www.blog.fehbvm.com/Article/details/gdgfsgegs.sHtML

[R68] 计算文件校验值
来源：http://wap.hesvh.cn/Article/details/gdnhnkimu.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fehbvm.com/Article/details/gkeocqvgl.sHtML

[R69] 生成随机密码
来源：http://blog.zdbjq.cn/Article/details/geynkaehg.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.zdbjq.cn/Article/details/gzynipzyg.sHtML

[R70] 时间戳与互转
来源：http://www.blog.hesvh.cn/Article/details/gnovmiwpe.sHtML

date +%s;  date -d @1700000000
来源：http://baike.zdbjq.cn/Article/details/girbkibxl.sHtML

[R71] 日期格式化
来源：http://read.share.hesvh.cn/Article/details/gpudnfctw.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.fehbvm.com/Article/details/gfpezjroq.sHtML

[R72] 等待端口就绪
来源：http://baike.hesvh.cn/Article/details/gvfkvbvje.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.zdbjq.cn/Article/details/ggwnbtnqq.sHtML

[R73] 分割大日志
来源：http://blog.zdbjq.cn/Article/details/gkfpkokoj.sHtML

split -l 1000 big.log part_
来源：http://www.share.fehbvm.com/Article/details/gzsfgxfeq.sHtML

[R74] 批量重命名
来源：http://read.share.zdbjq.cn/Article/details/gmxatrcpe.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fehbvm.com/Article/details/gahclhwxa.sHtML

[R75] 导出环境变量
来源：http://wap.zdbjq.cn/Article/details/gsxwfflgn.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.zdbjq.cn/Article/details/gxuxjkeev.sHtML

[R76] 使用临时文件
来源：http://read.share.zdbjq.cn/Article/details/ghrqmbwpw.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fehbvm.com/Article/details/gmkhlburj.sHtML

[R77] 读取用户输入
来源：http://3g.zdbjq.cn/Article/details/gtlponoon.sHtML

read -rp "请输入: " ans
来源：http://www.share.fehbvm.com/Article/details/gihzpwirx.sHtML

[R78] 交互式菜单
来源：http://www.m.share.hesvh.cn/Article/details/grsjfjpvx.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.hesvh.cn/Article/details/gjzojfnvq.sHtML

[R79] 解析命令行选项
来源：http://wap.fehbvm.com/Article/details/gicagatqb.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.zdbjq.cn/Article/details/ghdbvzgcc.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.fehbvm.com/Article/details/gqrhflhwb.sHtML

time ./run.sh
来源：http://m.share.fehbvm.com/Article/details/gqxlqrmzs.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gbdsitsky.sHtML

S. C / C++ 专题
来源：http://www.blog.zdbjq.cn/Article/details/grxubjkts.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gjakzolkq.sHtML

[S01] C：Hello World
来源：http://baike.hesvh.cn/Article/details/gvhwlhfhy.sHtML

#include <stdio.h>
来源：http://mobile.zdbjq.cn/Article/details/gfgvokony.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.zdbjq.cn/Article/details/gjfzhlzhf.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.zdbjq.cn/Article/details/gwjhjwkfk.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.hesvh.cn/Article/details/ggtzhmfzk.sHtML

[S03] C：读入整数
来源：http://www.blog.hesvh.cn/Article/details/gtsrbqoql.sHtML

int x; scanf("%d", &x);
来源：http://3g.zdbjq.cn/Article/details/gpibaqpcc.sHtML

[S04] C：字符串复制
来源：http://www.blog.hesvh.cn/Article/details/gomhojxqt.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.zdbjq.cn/Article/details/gozxfooyl.sHtML

[S05] C：字符串长度
来源：http://blog.fehbvm.com/Article/details/gimsfdeju.sHtML

strlen(s)
来源：http://3g.fehbvm.com/Article/details/grfmmykcq.sHtML

[S06] C：字符串比较
来源：http://m.share.zdbjq.cn/Article/details/giqsdspph.sHtML

strcmp(a, b) == 0
来源：http://m.share.zdbjq.cn/Article/details/gnqyurhlv.sHtML

[S07] C：数组遍历求和
来源：http://read.share.hesvh.cn/Article/details/gfnqamxtt.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.hesvh.cn/Article/details/gsxbkjeiz.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.hesvh.cn/Article/details/gpjnvsjsq.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.hesvh.cn/Article/details/gplenxnah.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.hesvh.cn/Article/details/gljrnonil.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.zdbjq.cn/Article/details/grauhyfpi.sHtML

[S10] C：指针与解引用
来源：http://www.share.zdbjq.cn/Article/details/gtoawvtet.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.hesvh.cn/Article/details/grkxopcpk.sHtML

[S11] C：逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gelzwmsue.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.fehbvm.com/Article/details/gclmobxys.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.fehbvm.com/Article/details/gusuoflrc.sHtML

fclose(f);
来源：http://wap.zdbjq.cn/Article/details/giasjjryk.sHtML

[S12] C：写文件
来源：http://read.share.hesvh.cn/Article/details/gkxejeetv.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.hesvh.cn/Article/details/gaqtntjpo.sHtML

[S13] C：宏定义
来源：http://www.m.share.fehbvm.com/Article/details/gaqvlbyva.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.zdbjq.cn/Article/details/gncthntqr.sHtML

[S14] C：枚举
来源：http://baike.zdbjq.cn/Article/details/gntavydqz.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.zdbjq.cn/Article/details/gbxqlxogo.sHtML

[S15] C：类型转换
来源：http://www.blog.hesvh.cn/Article/details/grxnfucun.sHtML

(double) a / b
来源：http://www.share.hesvh.cn/Article/details/gawuztzxz.sHtML

[S16] C：位操作置位
来源：http://www.blog.zdbjq.cn/Article/details/gxbcpcwbw.sHtML

x |= (1 << 3);
来源：http://blog.fehbvm.com/Article/details/ggrovzlxj.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fehbvm.com/Article/details/gxwusrcmt.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.hesvh.cn/Article/details/ghgvcudzu.sHtML

[S18] C：命令行参数
来源：http://www.share.zdbjq.cn/Article/details/gkvwbbfvl.sHtML

int main(int argc, char **argv)
来源：http://www.share.zdbjq.cn/Article/details/gzbyddkfr.sHtML

[S19] C：快速排序
来源：http://3g.hesvh.cn/Article/details/gmbjhjnyz.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.hesvh.cn/Article/details/gfgcrtuuj.sHtML

[S20] C：二分查找
来源：http://baike.zdbjq.cn/Article/details/glgmnaums.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.zdbjq.cn/Article/details/glvtnautk.sHtML

[S21] C：字符类别判断
来源：http://3g.zdbjq.cn/Article/details/gsbjgrukm.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.hesvh.cn/Article/details/grpcebdfu.sHtML

[S22] C：字符串转数字
来源：http://3g.fehbvm.com/Article/details/gphglwpab.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.hesvh.cn/Article/details/gvbpkiaxh.sHtML

[S23] C：随机数
来源：http://www.m.share.hesvh.cn/Article/details/glezxlmas.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.zdbjq.cn/Article/details/gxvmuffgu.sHtML

[S24] C：获取本地时间
来源：http://baike.fehbvm.com/Article/details/gzjmbxsav.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fehbvm.com/Article/details/gosfnxfrn.sHtML

[S25] C：内存拷贝
来源：http://mobile.hesvh.cn/Article/details/gllooeiny.sHtML

memcpy(dst, src, n);
来源：http://blog.fehbvm.com/Article/details/gjbnqicdg.sHtML

[S26] C：内存清零
来源：http://mobile.hesvh.cn/Article/details/glwrheexh.sHtML

memset(a, 0, sizeof a);
来源：http://wap.hesvh.cn/Article/details/ghmimzcyn.sHtML

[S27] C：定义常量
来源：http://3g.fehbvm.com/Article/details/gqnlnzrhk.sHtML

const double PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gvjbygleq.sHtML

[S28] C：静态变量
来源：http://www.m.share.fehbvm.com/Article/details/gonthhbco.sHtML

static int counter = 0;
来源：http://read.share.hesvh.cn/Article/details/guexengtu.sHtML

[S29] C：变参函数
来源：http://wap.zdbjq.cn/Article/details/gbskauaud.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.hesvh.cn/Article/details/gmzvhencl.sHtML

[S30] C：头文件保护
来源：http://baike.hesvh.cn/Article/details/gwduvngqu.sHtML

#ifndef X_H
来源：http://www.share.zdbjq.cn/Article/details/gwapqskly.sHtML

#define X_H
来源：http://baike.zdbjq.cn/Article/details/geknxtufj.sHtML

#endif
来源：http://www.share.zdbjq.cn/Article/details/gneijyunr.sHtML

[S31] C++：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gponushhc.sHtML

#include <iostream>
来源：http://3g.hesvh.cn/Article/details/gxseiofzc.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.zdbjq.cn/Article/details/gdosepibx.sHtML

[S32] C++：字符串
来源：http://m.share.fehbvm.com/Article/details/grktwxkrd.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.zdbjq.cn/Article/details/gnpeykojv.sHtML

[S33] C++：vector 增删
来源：http://wap.fehbvm.com/Article/details/gjeshtomw.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.hesvh.cn/Article/details/gtajfjexz.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.zdbjq.cn/Article/details/guzlbyhge.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.hesvh.cn/Article/details/gzdzireow.sHtML

[S35] C++：map
来源：http://baike.hesvh.cn/Article/details/ggumqzmpe.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.hesvh.cn/Article/details/gwqsirlgn.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.zdbjq.cn/Article/details/gqzvmxsow.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fehbvm.com/Article/details/goudasnnj.sHtML

[S37] C++：set
来源：http://baike.hesvh.cn/Article/details/gprvnqnvf.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fehbvm.com/Article/details/girlbpfrb.sHtML

[S38] C++：排序
来源：http://mobile.zdbjq.cn/Article/details/gdwlwsxnc.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.zdbjq.cn/Article/details/gcetnjlnv.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.zdbjq.cn/Article/details/gwzcxdfxp.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.fehbvm.com/Article/details/grioxhbte.sHtML

[S40] C++：查找元素
来源：http://www.m.share.hesvh.cn/Article/details/ggmmeehzq.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.hesvh.cn/Article/details/gxzjfjifb.sHtML

[S41] C++：类与构造函数
来源：http://www.share.fehbvm.com/Article/details/gvbdvmlwb.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.hesvh.cn/Article/details/ghjjfqmdb.sHtML

[S42] C++：继承与虚函数
来源：http://baike.fehbvm.com/Article/details/ghvqafpce.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.zdbjq.cn/Article/details/gkkhpvzil.sHtML

[S43] C++：智能指针
来源：http://baike.hesvh.cn/Article/details/glxhmqlls.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.hesvh.cn/Article/details/gboowfqgw.sHtML

[S44] C++：引用传参
来源：http://www.m.share.fehbvm.com/Article/details/gmodqozqz.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.zdbjq.cn/Article/details/gphqwddpv.sHtML

[S45] C++：lambda
来源：http://3g.hesvh.cn/Article/details/gjhcvdxiu.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.fehbvm.com/Article/details/gpgrtqmla.sHtML

[S46] C++：函数模板
来源：http://read.share.hesvh.cn/Article/details/gluccodne.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fehbvm.com/Article/details/gtvfoqxcm.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.zdbjq.cn/Article/details/gzvkotpwn.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.zdbjq.cn/Article/details/gqilgybfj.sHtML

[S48] C++：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gzozxjlap.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.fehbvm.com/Article/details/gxdrbhhdf.sHtML

while (std::getline(in, line)) { }
来源：http://blog.hesvh.cn/Article/details/gxzcjkqks.sHtML

[S49] C++：写文件
来源：http://m.share.zdbjq.cn/Article/details/gbvtajgui.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.fehbvm.com/Article/details/gljzhhecv.sHtML

[S50] C++：格式化数字
来源：http://www.share.zdbjq.cn/Article/details/grvdhvzom.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gtiartnvv.sHtML

[S51] C++：显式类型转换
来源：http://m.share.fehbvm.com/Article/details/gmfwlsnwe.sHtML

static_cast<double>(a) / b
来源：http://read.share.hesvh.cn/Article/details/gwnvqefys.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.hesvh.cn/Article/details/gecyjuiyg.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.fehbvm.com/Article/details/gwzkulecn.sHtML

[S53] C++：移动语义
来源：http://read.share.hesvh.cn/Article/details/gohxqxgov.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fehbvm.com/Article/details/gipvnthjq.sHtML

[S54] C++：异常处理
来源：http://wap.hesvh.cn/Article/details/ggkeiwudz.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.hesvh.cn/Article/details/gunckjuht.sHtML

[S55] C++：结构化绑定
来源：http://blog.zdbjq.cn/Article/details/ginulybsk.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.zdbjq.cn/Article/details/gwrkgxemi.sHtML

[S56] C++：optional
来源：http://mobile.hesvh.cn/Article/details/gsdsqdbqh.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.fehbvm.com/Article/details/gvpjukgaz.sHtML

[S57] C++：编译期常量
来源：http://blog.fehbvm.com/Article/details/gopqqeary.sHtML

constexpr int N = 10;
来源：http://www.share.zdbjq.cn/Article/details/gswevdlmm.sHtML

[S58] C++：命名空间
来源：http://www.blog.hesvh.cn/Article/details/gtyywwfhn.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.fehbvm.com/Article/details/gplwexfdd.sHtML

[S59] C++：静态断言
来源：http://3g.zdbjq.cn/Article/details/giscqyoxa.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.hesvh.cn/Article/details/getsupljs.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.zdbjq.cn/Article/details/gteenvfls.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.fehbvm.com/Article/details/gzztgnfqb.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gckmgqvsc.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fehbvm.com/Article/details/gjjifgzlp.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gpcgxgbxs.sHtML

[T01] Kotlin：Hello World
来源：http://wap.hesvh.cn/Article/details/gjimyzvhx.sHtML

println("Hello")
来源：http://m.share.hesvh.cn/Article/details/gmtawbycd.sHtML

[T02] Kotlin：变量
来源：http://3g.zdbjq.cn/Article/details/gbzapampq.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.zdbjq.cn/Article/details/gpcakqzcz.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.fehbvm.com/Article/details/gxrdrkkbf.sHtML

"值: $b"
来源：http://www.blog.zdbjq.cn/Article/details/gqqhgnqop.sHtML

[T04] Kotlin：空安全
来源：http://mobile.zdbjq.cn/Article/details/ghbvwpdue.sHtML

val n: String? = null;  n?.length
来源：http://3g.fehbvm.com/Article/details/gcfgkiwou.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.zdbjq.cn/Article/details/gvnaxbcyw.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.hesvh.cn/Article/details/gwhlcrrnw.sHtML

[T06] Kotlin：集合映射
来源：http://baike.fehbvm.com/Article/details/ghjhaedii.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.fehbvm.com/Article/details/gcajkatpz.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gkbpsiazx.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.fehbvm.com/Article/details/gjqyocgek.sHtML

[T08] Kotlin：数据类
来源：http://www.share.fehbvm.com/Article/details/gnqyoabgp.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.hesvh.cn/Article/details/glloyhjzp.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.fehbvm.com/Article/details/gebkyfbhr.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.zdbjq.cn/Article/details/gcxwcgbsh.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.zdbjq.cn/Article/details/gwfzywkqj.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.hesvh.cn/Article/details/gtamuwvju.sHtML

[T11] Kotlin：协程
来源：http://wap.zdbjq.cn/Article/details/gwncbjafe.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.hesvh.cn/Article/details/guhqbywzw.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.fehbvm.com/Article/details/gsvcnhkbz.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.hesvh.cn/Article/details/gjzuwlmrm.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.hesvh.cn/Article/details/gtyudciok.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.zdbjq.cn/Article/details/ghqoarwbp.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.hesvh.cn/Article/details/gmoplmros.sHtML

for (i in 1..10) println(i)
来源：http://blog.hesvh.cn/Article/details/gedqiywed.sHtML

[T15] Kotlin：接口
来源：http://m.share.zdbjq.cn/Article/details/ggsdugchh.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.zdbjq.cn/Article/details/gcfyudizc.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gqwzvnlzt.sHtML

print("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gntblebll.sHtML

[T17] Swift：变量与常量
来源：http://read.share.fehbvm.com/Article/details/gdckmptba.sHtML

var a = 1;  let b = 2
来源：http://www.blog.zdbjq.cn/Article/details/gsalrqdnj.sHtML

[T18] Swift：字符串插值
来源：http://blog.fehbvm.com/Article/details/gqzailigv.sHtML

"值: \(b)"
来源：http://www.share.fehbvm.com/Article/details/gyonfulpc.sHtML


<!-- 参考信息 -->