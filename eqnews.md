代发 wailian999

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2tclhtjfx.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2fdyntphw.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2fvnvwhwo.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2nnbqepwo.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2lfoahfxl.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2nwjklood.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2rqnhtgiu.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2cmaqsnja.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2fuxsekai.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2qxlncyqg.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2dbuzvfoy.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2lobcnueo.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2kcypkltn.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2kcopahir.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2pxjrxkwn.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ekfonams.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2djdviban.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2dfvojpqd.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2bfhyqujv.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2pojhwsad.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2rrzrjdhb.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2fouunbqi.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2byfyrgxs.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2tilflovd.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2yyskbynk.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2lxpxwvcf.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2mtvbvbrn.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2szbhapbm.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2ezqrxzpe.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2trwbiuax.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2iexxeewm.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2mywbrryp.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2wxyffvaz.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2dlnaoknq.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2mcxfjcvo.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2udfezcyj.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2btypwnpc.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2wgeshniv.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2hfwuvwcz.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2aemrhpqx.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2wqcqhdta.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2oflspthp.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2usgjdgzd.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2foisceqk.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2wjdwdecw.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2msedxxaq.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2yevjvrzi.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2fcvniexv.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dtnslwsv.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2upxivmcd.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2qhggcvin.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2wvkjuome.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2mfnnrcwg.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2fqxtlpfc.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2jhbyrcmh.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2qwurlvbd.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2rteixths.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2eujyhbed.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2nijdygla.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2rhfewakj.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2aduqdven.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2uibijzbt.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2qvzwrdss.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2hzkjkdzs.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2mlffqwjq.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2glchzvrd.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2ipmykguq.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2tdofzcur.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2qumoogau.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2ujjyvoxh.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2sumhwwgh.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2iauasmqk.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2gktgygoz.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2ycswsmjt.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2etddacnk.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2holxvute.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2hgiahtku.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2elhjfkjy.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2mzqnmgwg.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2xhykueed.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2hthmfkuz.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2jxfrunlt.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2wqyaebvy.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2sgkmunpo.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2tnaspxgw.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2ohwvqjaw.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2bvnpbxef.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2grrniuxp.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2xlabthkh.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2wiyhnglb.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2pyfabhwx.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2ffhhofel.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2dmvfsiku.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2hytszbfr.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2unhghwmi.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2dcosxxox.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2wkkyaviw.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2hoeqvdls.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2kqgnkhcb.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2zqboglwo.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2mqypemqs.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2zndkikyv.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2nijyxcoa.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2ujbktokw.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2ojotvrfb.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2jxbjdymr.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2gxzwcptb.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2xtbulvyw.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2ntcillxy.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2tulnnoaa.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2vjshxrgo.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2wltqzjmb.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2kgsjdkvf.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2oncqtwfj.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2ajqcmkmn.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2nulgvzos.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2mslvcznl.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2wiindwxn.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2qvhvrbao.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2rsfukwzn.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2wnkldfxj.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2caaaharb.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2fqdeafeb.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2rgjqoszq.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2dzmbmtij.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2allgeeyu.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2wullooto.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2extljgnx.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2iiorczou.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2ofyaskkx.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2ukuvjgqf.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2bqakyuvn.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2ucvasihw.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2qioslnjb.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2bdsqpzay.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2doacvsrr.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2fevytjfo.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2llcpmcqn.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2ttridgbi.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2nygkpkvb.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2gyxkprsu.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2gzoxsfsu.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2ovsuhxfq.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2crfroxjf.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2lltciekl.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2ehuccbne.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2xljyjudg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pbaswzwz.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2ybhhppyb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aekezwfz.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2hnekfndh.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2mspyrpfn.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2cbvsbcth.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2lwmvlvmo.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2drjthnhl.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2opykzatz.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2axzbuazl.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2ahzlutit.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2mwjjvyhc.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2sqoxwdue.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wwgkgqki.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2qkdusyyi.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2lyunbtaf.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2zmvaocjh.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2desnvhpo.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2nqvlaydv.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2mtnpbrzm.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2rhialfjt.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2hkpwqwbo.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2jwwtvrra.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2nmymzbxy.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2huuckkls.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2ajlknupe.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2rwufqcfx.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2zrdcsaae.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2cfcpkxzb.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2plujxdkg.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2kyabgvxv.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2oemsjhpp.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2uwplnjrg.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2rehpeppi.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2veamvqfk.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2thoxyhbk.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2nyeanlum.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2ljcbxssv.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2agmkdyml.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2ucocjrka.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2bmbkfjfq.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2okvajqor.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2prpeylvs.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2fcovdnpo.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2wgxltbny.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2javbhhle.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2hsxigtmq.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2hxcufkbj.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2ybuiisbd.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2cctktwoa.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2wuoqpzhx.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2zhxbsziz.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2iojtdnfz.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2tqfgyacw.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2vxnzjzqd.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2qmiftvpj.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2ecoshxtp.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2qkeazdfn.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2egqdswbs.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2vpnscbhe.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2fiuxhajb.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2bfgudcqb.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2mxubjbrh.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2wvfhqqrh.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2manyrwpb.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2ljehzkia.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2oujbwica.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2bzlydnat.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2efubzooe.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2fnputroy.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ghuccrlx.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2neopehrn.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2ocwysxgq.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2hquejecc.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2lduravmf.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2toqnxniw.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2dlfvaqjj.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2thrwaqwr.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2xvkbxhar.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2ptfyuckq.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2hantfxmr.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2dehxyrgl.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2hsyxuoia.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2vkndgswr.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2ksflhymz.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2msyheawc.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2mmgtfmal.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2srxltyir.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2cetipvkv.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2tiewndmj.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2ppaebucg.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2selaoewj.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2uilkixrw.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2brwnutnq.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2nqmqwnzn.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2endpbgjf.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2qqlwcgla.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2kdgvhswz.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2nprnufzh.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2oiurptoa.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2cswnqewq.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2aldodetu.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2kgrtwfjb.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2aazjoyro.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2tdhzkybp.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2lstlnzng.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2hutakhkq.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2mdpxlasc.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2calscvtg.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2yzocbnhp.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2tagibbfv.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2nlidoauq.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2gljpqnti.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2jtbuxvab.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2gniwqvzx.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2fqhsejqr.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2jbajyehw.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2uokijnfc.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2fpgbyxsp.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2jhracspp.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2qdyiqjze.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2nqynmcke.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2fmmwozpr.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2bqjeggwr.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2upsrwfyo.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2qtkqkdfq.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2oxayclmb.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2fstmesfx.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2owjsiove.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2jyvuxcno.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qecqbknx.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2tjzdhjvp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pqjqbjxv.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2aukwwvxv.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2tgvklrnz.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2izpxuspm.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2tugzxmfi.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2ncikznxs.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2clxnriad.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2blszjxmm.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2bbwzkzed.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2dicyjvlr.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2tvfgscgf.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2xuqbbozx.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2flgdkzjh.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2zcpvsqad.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2dziduifx.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2fnrvyyzm.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2inuhkedp.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2xyjeyfba.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2jgvtnggh.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2xvuqjxba.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2zazhuobu.html


<!-- 参考信息 -->