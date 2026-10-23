代发 wailian999

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3adehpouh.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3dlyaqozu.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3gnalrtjl.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3wyaxtroe.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3kdumljer.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3sedfhrgo.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3mcpsuqkg.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3krcayupx.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3uhclduqv.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3bwadltqn.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3aiocofhk.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3eeitngcb.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3hcrzenbc.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3ritszvfa.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3zzhcjwus.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3zgdguhgr.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3xtqpmzhf.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3dpneqrhg.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3vheywjru.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3poadiuzf.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3qnvmktfi.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3mcwuvbyt.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3xfvcmhdm.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3menejvpp.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3aiflilad.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3ppscnrqs.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3izainaaj.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ofjxwrqp.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3nxarqjaw.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3makwmfub.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3ndaqbimq.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3jdcudioh.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3ckwrfaox.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3tmfiecua.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3mjqvfgci.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3xrwdpghj.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3jbzvgmxf.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3xjedpwxa.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3ukxuwair.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3aygrmugk.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3clozthvo.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3wsvazihn.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3cdfnwivv.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3fiarzprm.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3ivtnyfry.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3ktqkanyi.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3tqakppwm.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3vchszlky.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3sqmrbjyh.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3mcfffvhu.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3hpqszsze.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3kvwunlob.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3wuhmcazi.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3qevbrqhk.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3fjbpamnh.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3lqbtqmyr.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3jzbkasfv.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3kleasytk.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3manavpvn.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3juurgwib.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ujteubdq.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3bpzloyso.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3nhcodlno.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3uqzqtcpx.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3femoinfj.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3vbaxdshq.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3hzawizku.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3vdsohuza.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3bubbxilh.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3chxqrpfa.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3tiaikmkl.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3xnwnbkpj.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3kaodlanv.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3kvbpazjt.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3huxqahbx.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3pjtwefgw.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3xxlkybxr.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3bzfexmcn.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3wgemjcuj.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3czaygbkc.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3mqfhkpce.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3lgqktypa.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3wslwqyru.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3zeyensph.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3nbcolzke.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3vwbpgdvd.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3ybzkgqhy.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3rztawpgi.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3rskucxqp.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3tsevclrj.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3ycgzwmaz.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3rairstmn.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3jqdhpvrl.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3vorkvufo.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3gmkrgptl.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3isxrscla.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3wkwmfhjw.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3vnnkpkcm.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3yirxcvgx.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3ynlirfmt.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3nxjmpelu.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3qztymrvl.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3kcweyyqa.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3yxnljdqw.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3ftzpdlyk.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3jlsmjbjg.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3rnfzreqq.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3edraalgn.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3rxkpomvy.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3vefhgnpi.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3tdlfvimq.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3mqngunzv.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3emkqfypx.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3ctaorgft.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3rervtwcx.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3efcgxwna.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3encypntv.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3kvvdcynv.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3olhvbflq.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3syvvowcy.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3yarpvscm.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3cvxavyya.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3ccwjrejm.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3cbwivegm.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3luezuhza.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3hkpsidlq.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3xrjrzowb.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3wnomqvuu.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3kuodqjrq.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3mehffeoh.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3nlszklwp.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3rjskibhm.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3xnemuwve.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3zcempusw.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ecualyqm.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3hnizcycd.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3gmhprwcb.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3drspfsey.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3zggjvsne.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3wosdfwzd.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3boxyddlp.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3sbzzoeqn.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3eoquphdo.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3egzxmlqj.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3vmlgvusk.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3artqbqex.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3hpdeznat.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3hpqmbrwy.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3zzbyvtca.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3hkzfyuia.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3nvrvyjdp.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3nvammcia.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3rliupzit.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3rjvnbxme.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3bucvphvt.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3pnflkaqk.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3flqrfjjg.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3dvmoabvx.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3rtjhrgdd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mraejaga.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3ndjaveiz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rbuxmubp.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3meuuobof.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3jysgqegr.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3iwmtklvd.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3jxxuogny.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3xkjfjwik.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3jhvobjqy.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3eyopamge.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3mnjwnbjt.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3zamxodse.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3urvoqyay.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3teiwkyvl.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3hbpoahzo.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3ifpfzmxm.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3hwycptus.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3ptkqfbst.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3yqhcjahp.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3xjpckrrs.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3qyliugco.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3lnzczjts.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3gtkcxopk.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3msgyarqa.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3hbhholvj.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3fyfmmfhg.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3pgpxgflb.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3quiifybi.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3ylifvmbx.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3pumslaan.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3uouwuvhh.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3nnojkgdd.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3ezitjuwn.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3rtekjgzc.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3lvyqkjwg.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3pkhcztfd.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3rvrkhugg.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3exqskode.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3jcbhdclk.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3erndsgix.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3ruxcjbgr.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3eofuqadq.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3nngzkieg.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3gtibwhia.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3pteejeml.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3jparlygv.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3sxewnjbe.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3iwtlaxid.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3rpqcfspi.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3iskzcdky.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3xdwrumta.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3wstacxqz.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3ctxobcqf.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3brrvaqro.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3aeplzmyr.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3ugzgntgm.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3irdwjwtu.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3ptplnljv.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3umffvxgl.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3leombjqh.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3xajnphke.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3ouycecjp.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3hbjjtfrn.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3ifohjgcs.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3biirvknq.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3sjkvkoay.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3iycbelpa.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3xwxxdzcl.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3vknkbqwy.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3ydreyndg.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fecnpwmx.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3znuvxdmx.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3gotsirrs.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3lpbtgdmd.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3vdwoqxfk.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3bzacexol.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3srbmtrlz.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3sdkzfilf.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3bddipuuo.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3dqaplqnq.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3zagctxgr.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3ujlzoodp.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3ddvdshpc.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3rqklpgxy.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3plpcydoz.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3qprmyzkp.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3srzsvjau.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3yjmfjnvd.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3feyfqbpa.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3ejtjcwlh.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3hgvxnikp.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3vnmppwsj.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3ydrdtoen.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3msliitqj.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3nfziyjyg.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3acqnwuyp.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3aqgbxewp.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3wgpatcin.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3bjfwmgic.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3pfcsjaeh.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3izzorgdm.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3dmvwbcis.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3pbyizple.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ghwgbkqi.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3cpkhdzmg.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3hwezxfek.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3ndjuoovx.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3kgfbcegk.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3mseswawo.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3xnkaerws.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3royushij.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3lhmithei.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3wtarbsul.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3ktnhzhax.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3jnkkexur.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3nmuprscw.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3ewgqharh.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3bjfnybfn.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3umrggdes.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3grulcebi.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3ecgayqys.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3ihsnexgw.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3cqnxvoso.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3ocochcut.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3emybebkx.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3flvdxlyc.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3gibjbnhq.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3wyixnugj.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3vadazhew.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3wfgnfuvu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iwavwnwc.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3wvriaism.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jiwnyrca.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3wsdfzyoi.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3thhutzqu.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3cdoomksm.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3mrglauts.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3nozmzswt.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3yvvafteb.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3eajejlai.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3juzfsfni.html


<!-- 参考信息 -->