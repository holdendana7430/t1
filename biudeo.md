代发 wailian999

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2gadijljw.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2rsjcoicv.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2riwgrske.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2yqhwlxsc.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2sdotvauk.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2tuedcmjk.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2qgicruje.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2imvegzfi.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2kzfohorj.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2obybowil.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2wlcntcas.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2dptsjgro.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2twhrztuh.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2lidotwov.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2nwedhems.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2qwbgbevp.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2eazuetkw.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2unovpnlh.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2jkcyqsmf.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2ixypdgat.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2eankdvdn.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2afaewhut.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2qqnnkifn.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2cfedopty.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2qvvlteaf.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2tmhjtzpc.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2psxdmvhx.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2awxxfqik.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2xhtrzgub.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2pjphswsg.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2chszrxxg.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2gdttbpcm.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2yxitzsxr.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2ygtmcvbh.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2dceaavkb.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2ujnkldrp.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2uxourria.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2cmmxwnqw.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2ueavoyma.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2tvabaoyd.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2nkiotmzb.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2odeiritm.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2mumcsdxo.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2mrslhrih.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2rdhrngwx.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2gzapwfxf.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2rekvzghq.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2rmphinfz.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2lauprzll.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2jadkvsvt.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2umpciwvp.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2vzguahvf.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2xqrzlirt.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2iibvwgdj.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2skyhkbhc.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2bbnhaora.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2qwdsweri.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2pxoohhvf.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2tsbfuuvd.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2elkskggg.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2hrrpwpfz.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2hcgiswwx.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2urjkvtqm.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2jucmkzoi.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2ejfkdeul.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2rnvafbkb.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2tmeokbmm.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2slhtvmsy.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2fdispzye.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2tegavyje.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2vxgpkbdg.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2thldsfqp.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2cldojtdv.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2mccwraeq.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2kknjumgo.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2kxmptxop.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ejpdkbhu.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2dlqdgkef.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2igtmrpia.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2pgylmmpr.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2ljgfrbea.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2kycomlzl.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2twapphqx.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2svwwprqf.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2qlhezjzs.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2pkulpkqt.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ujbenuma.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2rysggqta.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2zyuhlcnx.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2gaztvmht.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2buwbtuvl.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2grmiijpc.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2pblezbsj.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2afwjnipl.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2iyauvsgx.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2xprmxorz.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2jnurhgbr.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2sqfoivke.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2tiwrttyc.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2svisinrp.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2naxkwzqi.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2cdqafdrp.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2yeceaaer.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2bhcyiina.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2fymcnrut.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2djqypycd.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2akqvgzbj.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2pbrzvszd.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2untgaqxg.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2ynldhgkm.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2twevhwig.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2axmaisga.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2dekmeqio.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2krxufjkf.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2wohyidou.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2whmakrzv.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2xvrjdutd.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2sxdkeacl.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2maocfxdq.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2pqwphsfs.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2pvknjeib.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2noacypab.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2stldglvx.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2pmbmgwud.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2oryqpvkm.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2qulbcivl.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2srpeyfpi.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2tdjsilao.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2gnlmbaar.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2kkyvovwn.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2ujjqpuxv.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2yyhbpzcn.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2zgeosudd.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2ewjpxghh.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2tfkfbqac.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2hpzumbnv.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2yssihvox.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2rwhvpmye.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2pxpiuxuh.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2ruiylwmi.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2lgemmfzl.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2zteckbgt.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2jozvtduy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2svwwjjda.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2lletegwo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gxaizxhp.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ztiafula.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2aqidbgjr.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2dywaomaq.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2bkijnnek.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2nautwhum.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2lewdcaoc.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2lpnfwwwq.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2pizlyona.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2zoolcagq.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2tihrgvda.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cqilmxud.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2eruazzui.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2mjefqpyx.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2xzhehjut.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2viigtxqb.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2offuazzh.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2hrxgkhae.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2mqwrvzil.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2apshqrcx.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2othgxkip.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2ngygcxwm.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ihulxpgd.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2cshmdliq.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2ngpwbonn.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2qkhnbdey.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2pqrlxcsk.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2xnxthyix.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2nyjhcpnu.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2pvcdbmtd.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2nbzleuis.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2jovqlwko.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2idoaxoul.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2pzzznsyx.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2plvlmmeg.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2bgkpscsy.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xdhxujdb.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2yyrdjepo.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2dxdxuhtg.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2btxfqqlh.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2aoqzjycp.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2drbbsdal.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2gbbivrvu.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2ovwtctyv.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2pojmvgze.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2osepsxai.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2irhycmov.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2agbkygeu.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2bdurskfo.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2ztwrjhqm.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2ybcrzaxv.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2obwlambz.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2apljjyry.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2ekbsykcy.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2zqamrtnn.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2xhueojcw.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2plqsgxni.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2eqkgyxwh.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2kbnuibcb.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2amhnmhba.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2eoiqukdd.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2yxwuinyr.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2qtfurusg.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2bkuvljxg.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2gmkhmtkx.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2vaomjlvu.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2hgneehet.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2hbitpskv.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2drgatlpi.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2sczgeztv.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2afrnhamt.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2lmotezen.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2gglyjhrs.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2dwbwbmep.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2ltbdfecr.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2xkhkzwge.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2dcvyguss.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2nicezmha.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2deejumps.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2xoljeuhr.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2cquiofmd.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2tcobwtmg.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2olsjixoa.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2vstqswzf.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2ctcwhnkh.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2sswspunu.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2mmxsxdpn.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2isrucgsb.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2azdsmerc.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2bfwrrcyt.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2nounrart.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2nuleoqmf.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2ieqzyrfy.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2eryagsex.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2rvzdikao.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2xlmkyfxw.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2qwvnulcd.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2kukuyaex.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ajjydhri.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2xnpwmzjf.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2xmisbtym.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2yhgqwsqa.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2kzttcpxg.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2onhltecq.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2btjpnpui.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2ghxzqzzi.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2dhfrjqjl.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ingvgylt.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2sspoducq.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2fznsedxl.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2ikcjbvmv.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2wpjpvqig.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2hsstgsrg.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2kexwvune.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2milfvmhd.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2lexmmtga.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2ahepemyd.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2evxhdmcn.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2ejukltir.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2dfswfkax.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2djvjaqlt.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2ngnddotl.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2zqwqneky.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2iosjotrz.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2iagoyhhg.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2cnhzusof.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2auxmakrb.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2ajkwjmga.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jtlgngry.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2wuxfpmrv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dvgsdord.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2balrvbpa.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2acjrwfpf.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2oodimvye.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2mumtgbyy.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2ogsoehfr.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2qvntwpuv.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2txyxoaxu.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2nphwhxig.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2pawojnac.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2hssdxjjf.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2evvmaabp.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2ibhkcgmb.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2vyfsymap.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2yycrgeur.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2exqfbotd.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2omfqklyh.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2pdquedxe.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2dczxdqog.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2qiqzxnym.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2czpqqfmj.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2acbnuvnz.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2fxyeujjz.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2nhkgspqs.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2vnvsezko.html


<!-- 参考信息 -->