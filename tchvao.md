代发 wailian999

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2iahrycba.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2gdgmftam.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2jujyhtmc.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2vkakuqzu.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2azrctynm.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2obfgxqvm.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2dhbsoyrr.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2waevrxnx.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2zllyekci.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2lycdsili.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2gjqgtabh.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2qcxnpkfq.html

esac
来源：http://www.52xcode.cn/Article/details/gt2dozcqpbh.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2jdkfvfov.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2kkjblxtg.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2gjafflka.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2kcvmyarm.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2fnngbxgb.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2rxgfeptv.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2mzqdetpc.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2dpifcmhr.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2mftteqpn.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2dvjplptf.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2wasekbha.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2mmfghuan.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2rvwcggub.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2ymbgpqfd.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2mezbgxvu.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2pfmuytju.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2hmxcthqs.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2plvefxln.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2uswhffzk.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2eaoofltf.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2esqypddc.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2ojncwpwq.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2hiyskzxv.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2froiazsj.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2erxtwpfw.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2cvczkduw.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2jexwvjgc.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2vpuwyefz.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2csmbrxhl.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2temtdyth.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2twmedawq.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2gseidcyu.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2ncelzbqp.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2eczddzlu.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2hwmejddl.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2zeglzjgj.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2bevuvnbd.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2seaoxkpl.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2dgostlhj.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vjzwegjs.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2ydroyxsg.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2vdhjlunm.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2aaswzhbm.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2obcbfngf.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2jbedmxwa.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2ezknccwh.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2jrikocac.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2emqtwlir.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2hjjdpjvc.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2lcvmeuhe.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2ccnikcym.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2cbyifler.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2gzjjqiyl.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2jjnsnqak.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2sgpelpgk.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2rduqxfuu.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2qhdrzvvd.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2bijntphn.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2fstceyzg.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2hzgdrxam.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2nhaewofa.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2pvwmxbvc.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2cyvunhnd.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2bgiphici.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2twgeeqlz.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2kbmbsagg.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2swtqcahd.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2utnhvxfu.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2dbhovlcd.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2oqcgillh.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2cetmxzax.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2swycpfpw.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2ygbcetis.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2lwmalkbz.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2wiryqvzn.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2muvqusyz.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2negfwzrs.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2uouyzmou.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2gobpuave.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2pcuqoknv.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2loqslonm.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2hkyubvgq.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2iouumqij.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2kcdfstzg.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2hsdjsyvs.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2adobiyoi.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2lwzmzfmi.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2hrgywecb.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2tslkjlru.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2pckvdtgb.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2vzlrqblb.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2jvhqeiak.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2wgoteqkg.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2jflzvbbw.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2qoewwfxi.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2vprnpodj.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2uohhtfss.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2gcewzers.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2uybdqknc.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2dpcvqwpd.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2nxckbuos.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2vekqmbve.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2obempbtn.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2gtxxkphf.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2yadpijsb.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2lzojanrs.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2erczufuj.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2imbeaimg.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2sdofvguy.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2uxvivifc.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2exvqayfc.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2brmrjbpi.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2xixkckre.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2urtupizs.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2yyrlejnh.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2sxqngbsy.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2unaecbwy.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2kxtbsnwh.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2xuranqmg.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2rllyptem.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2ufubxelr.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2yichecqo.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2nmvawazr.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2seyhmxkq.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2wcwqwaka.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2ugcixtvc.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2qqqcvgqm.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2xwzovcjv.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2kbahoawk.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2jgjvchyp.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2sphhxujz.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2hosjzelt.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2ffhjgisl.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2znelpper.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2dclxmbxb.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2juzpqkkk.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2ebjeuzwz.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2tcnsbajx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oygatibb.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2blxvlukp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dszqcejy.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2dmfnjsxn.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2qqxmxmbn.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2mjijjsrq.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2bxxohhdl.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2xxeqhgry.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2vnpedigu.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2jzdtuwxn.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2zvjhumpa.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2dfsfrzlh.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2zfbneygn.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2nuuzlqen.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2cdkquqjb.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2gswphhqf.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2kuxhkwqf.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2vaebwutz.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2wbjupzqf.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2libpjpbf.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2uckhsqif.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2axornlnd.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2rgqfshgz.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2tghwejel.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2mxxdxdvb.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2kebwbltp.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2ztqmeibj.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2gqxpfplv.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2hcsxvscr.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2yxagmmcj.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2oyrkwvzx.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2amhypges.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2qebaeqgd.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2kvovkuxx.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2cyuyftqd.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2ytmzdpwi.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2skomvojm.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2mxybgtor.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2lzjdjhku.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2dadbonnl.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2zfkihaze.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2ktznvgnv.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2esypimkp.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2bfrutgal.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2mpqveuqj.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2lkcewpnd.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2bcumlkhn.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2spmvmvfe.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2gtmmpqyx.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2ujzvfesv.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2yrxlqout.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2womoibyp.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2xkbcekdc.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2jttvtgas.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2swdduici.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2gaeuadxy.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2hyenibrm.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2vfhudlkg.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2feguesdh.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2fukhrjsh.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2rizcxazd.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2amrnlyrn.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2jqobpihm.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2fkrfbtho.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2rfsuecqn.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2cumtjeci.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2lfzymyuk.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2htsbbofi.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2mqxojmos.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2jvvqzebn.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2fxnwvwns.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2lhyuqhwe.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2bjotqzer.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2lmhfyfzg.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2hvewleur.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2bpwkjizz.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2hoqjdedc.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2fdoouque.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2hbeewucr.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2xrixxbwv.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2kfytjqkw.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2yeklhokr.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2xvumjntz.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2xyhlnbtf.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2vaxafvda.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2apxchfla.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2oagbgpdo.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2fmavhebh.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2jkdjhmdb.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2kujtybum.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2tstwrhnf.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2evijyzgp.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2cpashqii.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2tmkovjjs.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2sopwizfe.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2maduxupn.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2blnwyoxs.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2wwjvvioq.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2znpcxwnn.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2aeeiuhdj.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2vwooxrqo.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2clmlaypt.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2xxugyqlp.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2kmimtuaa.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2vtkjnyva.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2aqxztjto.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2hndxdhwi.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2ijulwtzj.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2uxznpkbc.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ovokewqv.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2bjolauhg.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2tdqhpfcd.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2rvlfcmzl.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2inllnqyj.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2huxwxmdk.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2wirhjtui.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2luvriszd.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2gxqxciau.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2lqtaxqoy.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2rhllnyeb.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2jrlvppao.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2klbqvtet.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2ctnbnday.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2ccinzkop.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2mwgijbjo.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ygcoirvf.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2fnkymivg.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2ictnefij.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2cyztlidg.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2motppmcq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dathttqc.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2yfsxxhnh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lnhsebao.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2gxoflxaq.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2cmeqabyu.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2suavlkse.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2znydfhkg.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2leprxkoc.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2yrqlzvqs.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2bcctjphj.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2phqpmxvh.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2iyfuxrbs.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2frdwhqdm.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2nyykuhzk.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2jujvzuou.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2sakjchca.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2jketxnbj.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2fxhaytsm.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2zmhcnysk.html


<!-- 参考信息 -->