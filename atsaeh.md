代发 wailian999

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3jbuxhzjw.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3xtciqihv.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3bvzfgphz.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3axbbjbez.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3bncvnxlz.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3rsmncfqh.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3bzcsbmzp.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3mlyeztad.html

esac
来源：http://www.52xcode.cn/Article/details/gt3momjgjim.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3zjrbhhet.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3zqzdqeqw.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3jphnghck.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3lbhlzmur.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3jgnbfwne.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3iwppmhka.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3zebufhgp.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ogbnajip.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3wgjinlzg.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3rbfcxdrc.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3dpehoosl.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3musqtrbs.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3bzgqdawv.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3bmxmvuxn.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3mnrmgxzm.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3qpxpbuld.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3ybqtfnmm.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3voayfzbe.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3xazejdfn.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3vghltdbl.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3qqlwlfba.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3lpdcncmf.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3qsswldwq.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3vizidifr.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3ukqlswog.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3sghbgzpl.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3ooaryzfu.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3bvabszwy.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3qzcpzllu.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3tkywjrcu.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3kgcrkjtb.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3twrtakpc.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3itaqvmds.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3creffamw.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3hfdonqig.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3vmysmgzb.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3ugeavscq.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3pkjkzcin.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3qxrfzzcp.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rjcgopve.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3jsbczeuc.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3iufbhzoe.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3phlpbglx.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3hduoezli.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3rqoykxub.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3vohbtzpj.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3ecwurijn.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3pywlwuig.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3vbdjtmhf.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3pjayteyy.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3wxzwndxr.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3hkkxucwp.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3bozdrrqu.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3gvagrroj.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3ucoonmot.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3cyiwbgmi.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3clofcljr.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3ssgwsmsk.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3phuiadkc.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3xfyzhtst.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3ybvwgrbh.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3flauasab.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3djltivwn.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3kvscmlir.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3bzswhfmb.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3kvnrhsmd.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3uwqrviln.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3arkzbgzb.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3vdwwdtxz.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3usqcvjvh.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3rluqhwhc.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3rpbeoifg.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3oujeckre.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3ahlidufe.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3rxogjesq.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3ibdzviuy.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3uylsvfsc.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3sethzefj.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3revwzkyk.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3lxacrcsz.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3ufujsokl.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3xpoaxoyp.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3spfseick.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3cfkuvhkl.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3xawledbs.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3tkkigzrv.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3gimtggwl.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3mdvangzh.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3xsdklhse.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3bavyejce.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3medqswux.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3tooiktbu.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3znvgdqwc.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3onvjlxoc.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3jkzupxfi.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3uvtrmvoq.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3nivwszht.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3grdnpnab.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3mifdxrcl.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3zgprhsab.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3tvqalfqk.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3fcpnchob.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3ybpsemvx.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3pdviofyy.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3zaycfsjp.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3htqcfbro.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3aqreomgs.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3mestwpdc.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3gollzwgb.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3bgouxtfb.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3gzvvcjfu.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3memjoaoy.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3abkrvits.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3qwibmvsa.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3byklikvv.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3ynnikgzs.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3nynlqzot.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3iqppybel.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3uyndtkta.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3onsfietd.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3vllxrjbd.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3gysqwcus.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3kaphyznl.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3sjxbqvhu.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3wdxgprcn.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3gtqdxyjm.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3tkcyjasl.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3epfjoyih.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3dfoyldjs.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3jpxbtlll.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3dvitfmec.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3erwllweg.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3ecaadtxy.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3qsfnzkvt.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3ngfxolhv.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3pxewspmt.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3mmrxbzvl.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3vkemvjes.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ghtujghc.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3zjeeejqo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3drmimgaq.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3jyujcjsz.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3ljldjvhk.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3rkebwhri.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3qmuqfuwv.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3pgwsivbl.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3gzzrhblf.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3wvzbavwf.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3bulzctxj.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3cmkvugrk.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3jwcrnxvr.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3yqzulmos.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3addttlus.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3ehobambe.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3tbpxkueu.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3esyngxpq.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3ceesstio.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3icyssdzi.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3uyxdugfg.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3crgokmwc.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3lxowzoyh.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3vzrgwgpm.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3farnwlhh.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3qbwrqmai.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3zstxzwdg.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3wiwrgiwd.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3ejqetnwh.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3rlmmzyah.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3wrlchjvz.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3iqyoautw.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3cblsstay.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3zzvffgbs.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3rhkzjqdv.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3afoucnsl.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3phzmzycg.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3kqfjovzw.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3mcovdehf.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3tircsisz.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3opxpclug.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3gppbcqur.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3amgwncqp.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3pbvontxb.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3hewtmutu.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3vyszluah.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3ltrhsaop.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3rvtsnlsl.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3haexaqcy.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3crxrngsg.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3ntvipaku.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3nfctzibr.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3okayjpih.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3qbxdelld.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3gjzretgd.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3dfrgmscs.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3mnoglujf.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3atgpdtev.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3ruejgzjp.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3xqbhzmxw.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3gimhcjqt.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3exbldhvj.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3ulaseerj.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3rkkyujlf.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3ohlzaldu.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3istfoavm.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3pelyfcnl.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3xjncjzye.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3nvhpslsf.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3ztcoeqfp.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3oqkqiuxf.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3kxsvanqm.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3auaqcmyd.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3ftooyjin.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3gdwfeteg.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3jvaaxaou.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3hdctyaua.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3cupdsdbd.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3dkriyzxz.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3ismbvdxu.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3aujqmbon.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3gxdflbbl.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3xvmsgpym.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3zabukyok.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3goruyblf.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3gvxykxkp.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3ihamaqya.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3zdipzljo.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3krqdwqej.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3bwveohor.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3ssltrmrj.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3vndtzktw.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3ddkclprm.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3bhblhcto.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3ckhhvjcf.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3nqxrbkps.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3vkdrzici.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3lankafha.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3ovporwnq.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3coobupqt.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3jwiajxic.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3zidkztet.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3piunsnmk.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ddzrdbvp.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3saevcuwk.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3insesqhb.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3ccptlqij.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3ipuelpxm.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3dqgczfvh.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3bcbmcsxt.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3ackuzgru.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3qtjjgxcu.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3gznciuau.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3loxkogdz.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3nlmjlvsy.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3cfoqhlmc.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3fewhzgyl.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3ljkrzeii.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3nskyprvz.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3nbodcffp.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3kwwcdgea.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3pjufglvp.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3vymdiyst.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3hlivfuzs.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3mwrqldbr.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3arotbuaf.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3uwhakznc.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3iqaabzjk.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3pxfmzfcz.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3xpxqhvpo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mkbnlngh.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3kjuvrprg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fbkseons.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3pljqfslj.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3zxlgqsdg.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3uljtgpoc.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3verzcjyk.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3obhynggg.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3eolbukki.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3gjoysmnn.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3zwcbfruq.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3cgpcljkg.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3pjiwcgpw.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3rzmtgffp.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3iyhabodh.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3sjyynaul.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3japtcnbt.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3ggqxwjqd.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3xqbpxhde.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3dvphzvll.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3muucsymc.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3tzqivvbb.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3nkrhofct.html


<!-- 参考信息 -->