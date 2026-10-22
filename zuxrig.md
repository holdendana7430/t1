代发 wailian999

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ykzzoizf.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2grajjslb.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ecbymzvg.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2liusrvbk.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2eweplsci.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2uuchcfft.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2uwlwezvc.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2yfozozye.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2ommtfwpz.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2oiszinus.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2fhavotmr.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2lnydlpwb.html

esac
来源：http://www.52xcode.cn/Article/details/gt2ekampjvb.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2iwnpqycf.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2jdlsvxcl.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2xkhnbcuf.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2psvzqayh.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2iebsoppf.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2jdzaiyrb.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2ubtwhbeh.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2neisqytp.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2zbauesyl.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2cjstiotu.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2tvkzbxjl.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2ypeofvrz.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2zfjjtppo.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2sfdarbdw.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2czslkblv.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2ozfplpfk.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2agiploea.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2wfcimznp.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2mbpxeepa.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2lwcphqqe.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2ituijdoc.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2qcmfmzgl.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2cmokzmxr.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2tqjknuft.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2qmljdzve.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2buzvpzcw.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2jmoewqwq.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2uetyzuot.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2fjcrooah.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2jwlvfmsp.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2quuaxisu.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2bdffwfeq.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2cgtgrvfv.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2srsxhtfe.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2cjbzmxku.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2vopgyzep.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2mdwxkwmt.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2ijquspro.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2kadcautf.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2btisrzau.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2wvpdschw.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2bdaphlpz.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2cbupqacx.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2smpkosmh.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2rlaxrczv.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2cxudusip.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2nwcpdhzu.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2ctekgixy.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2ooawvnev.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2plwshjll.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2edkhcedy.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2rngiexta.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2uhhxaggm.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2srureflb.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2gwseokbn.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2hohcregc.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2sqxstbca.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2rpghovvb.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2zvensknz.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2bxgqwoyf.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2bzvcvcgv.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2khlesyyi.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2pymedkux.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2sbxckosq.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2umfmonxn.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2xbhsajjm.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2amkxgyzm.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2moeywkgc.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2jcqcbrrl.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2dggwmztn.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2nxdgvdpu.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2htoptxvn.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2xlvelytz.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2omvibytg.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2rxfrewsf.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2dsifztar.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2dvhuhyms.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2wufxvhxw.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2gffxfadg.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2umzgweiw.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2tyvnosiz.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2avwjnjcs.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2sbxpwbfj.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2febfwzyw.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2pqlwimvl.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2hplmvxdc.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2jrpgshok.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2avdatcdg.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2reylcukj.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2cjkqcsqy.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2hadbrdes.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2lnwmzfkv.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2wmrokzql.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2pbbmtbdy.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2oaobhjvz.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2uuzsaxqb.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2whvyezbk.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2stbbkmdx.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2okvykljn.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2ifwuzjzu.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2kzssbpac.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2brqthezq.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2kuaslhwr.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2fwbqvtnq.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2pkdhndge.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2dagoexej.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2niztxkjs.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2fchjmtdf.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2arcvyvmx.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2jgvutcyo.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2ozunjlac.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2lwpoleqq.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2ncywnxqu.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2pukgwldc.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2btqxsqco.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2ejopurjz.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2npjtsjov.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2kfmhsqjj.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2okqovdrz.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2jsxvfmcd.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2arbeekxp.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2wzmmsqja.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2dfythchw.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2erqyfjmk.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2rhhjscbs.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2rkpcmrht.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2sifkslmh.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2seuxcikd.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2spbaonjh.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2zmgrmdxu.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2gipbdoow.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2zdpfvmjx.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2ihiugfvb.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2fqpapoql.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2viggcbeq.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2vdsafjnh.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2pmyfvfrx.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2gkvnfmyl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jdpmgnfh.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2dfmmyjqd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wklbuiqc.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2wtdtfydd.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2aumdsbwi.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2oiqptzzv.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2oyalhiii.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2tyrjhohd.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2tgsefjjk.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2wwtirufh.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2axucknur.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2vkxinroh.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2rvffwlkr.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tkoseeyy.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2oxmgnrvx.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2qwrjlswx.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2ywlnaugp.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2rykpjfvh.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2zyonfjpf.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2nbqikwbj.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2mujqnelm.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2eudeypkd.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2znsbzcrx.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2wyfgijnn.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2wtwwcuex.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2kzynujmv.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2ntglyobl.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2jzdronrp.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2gfwoxmtc.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2mcyeuchb.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2nhbqdwlt.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2mxmyltsv.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2qepowoes.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2bdvcjlmv.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2crxlumez.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2zctvpwjq.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2lrzlzlsg.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2rvmthwje.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vosklprk.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2nivokqtn.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2vxqhlxej.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2uqyouzno.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2vihpbjts.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2havkdnud.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2eoalvkwu.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2sxqabjyo.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2ioylsplh.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2hypyvoag.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2swxtkqcb.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2npjbufbg.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2qxmbngaf.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2akwxpmsb.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2wynbuosl.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2ibududst.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2omowbvje.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2jjbaibfo.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2hvhpufjv.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2hifumobd.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2kwvuwhlg.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2lpoguuxs.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2jfjbcvaj.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2cjixqwxk.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2xtvcmrrn.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2xqysssct.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2ejryszbf.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2gxycqrer.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2thevdneu.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2zazqveec.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2vhurvcfj.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2thkdjyip.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2eughvznx.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mndabokv.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2uwwohwhl.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2kyzsajzq.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2kytsvxov.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2woozjesd.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2urphzjvw.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2khgpbbpa.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2qrwdvokc.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2bafhhmzm.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2sktffpir.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2ryyzrcnr.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2oqxqqnvw.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2nhidlyxx.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2pclxmiae.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2jjmuujxp.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2eqhjzofm.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2uhrbfdqr.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2nzqfxxja.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2etlwyars.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2qrvfawrm.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2wfkhrclq.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2curbzwdc.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2ryfeyvhu.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2zutpeoob.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2ddgynxpg.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2edzbwidk.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2jemsfhex.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2brrvxfzp.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2qpkbpnwx.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2fbxebent.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2jfpaxwar.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2ffwcmkxe.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ntunuftx.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2kwznbaob.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2vbzeehkz.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2ocntmvmd.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2nxauqund.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2gcamrguy.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2censoznx.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2ulktcrqc.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2nmaqahww.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2wkthzyro.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2zzvftsqc.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2gvduesle.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2swkkpzjz.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2cvrmzihe.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2davnijud.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2pfgqqlxs.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2daqjuihh.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2vntvibnz.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2duwuxxcg.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2ifiphipj.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2cnygqpcx.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2qmhfvddc.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2jsmcxmvv.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2wmptmbjj.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2tifabtod.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2akboinia.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2lyyecosn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jwwziasp.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2xugwpdph.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ebzpcnrh.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2hdkkpkij.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2objyraad.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2dnovdxhu.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2lwkgwxda.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2kyhjpukv.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2muvhbhda.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2plnhmtsi.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2dlwdmsfm.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ahwdompn.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2itdpnedl.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2sqcawoff.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2cigbtgfq.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2klywywlq.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2bqeskuuw.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2uyzwgala.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2ndlsvdad.html


<!-- 参考信息 -->