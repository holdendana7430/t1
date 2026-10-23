代发 wailian999

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3utvlohhm.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3uufdirxc.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3nfwwffzk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bezbflnn.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3tcymilik.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uskcmxlb.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3mwmprwqz.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3sgtblnbz.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3zqzbscct.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3bmxkmmbq.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3tdhcyigs.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3pvvolgrq.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3gxdxgyix.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3lqzbtxya.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3geanktpw.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3kqgqqlts.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3tziewbwe.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3gtcqjeks.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3vgjyfkwz.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3jdfajzkc.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3bvmeirjm.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3zfaunjlb.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3nhagshwj.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3skuopvnc.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3yhcxbzzg.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3bdnbivxk.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3zkbmvpwi.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3zxhwkfed.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3rjxggqmf.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3mcsjayhc.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3moygvygx.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3kuoqlvqc.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3fvzkcdhm.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3bhmkwbft.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3pvlmuevd.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3yrfjwlhb.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3nqirjtjl.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3hyzqfmif.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3hegjpgmx.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3wwwqemmx.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3mswkmfzg.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3ucjbwbdi.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3gglawyae.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3leoxvvvu.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3exhzlhdn.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3jqeaaswk.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3rpncuqen.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3vwzgwvor.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3xsjwtqgq.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3rxtimqfn.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3xjhvzjoq.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3jchadabl.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3cbrnlzxw.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3ipvpihep.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3urukgipz.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3fobygsua.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3wpacdzlv.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3dltagovw.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3fhdtejdd.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3ojnszzcj.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3hdsnytlw.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3gnyvykhb.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3axxgvvwc.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3vlkkikql.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3cwhxvudp.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3nbstcvnt.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3uhukphbf.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3brwuqmnl.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3vwymxkeo.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3gbbynyes.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3opsapolw.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3zvxiknzo.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ewmhovat.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3xxnplbew.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3ozuhhqug.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3gzvejnfy.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3hlvatxqx.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3lqzjuphw.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3cggnznxk.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3fyosjyqo.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3ftffzwlm.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3zsweeilb.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3feabnpgq.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3rfdvuvzf.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3bfnyzfds.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3ruhnglce.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3slgfcatm.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3optjpova.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3rziafxeo.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3kfkbeggr.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3azlxvfqd.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3pixopmeg.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3yjzkbved.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3suuflivc.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3adgvgamj.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3zplmjhnz.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3xbpxfnwk.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3ugrjprof.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3qmogfcxm.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3gtyuuqyu.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3ceazqfnx.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3lgjkmzpt.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3sgeqthbc.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3fusgmltk.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3gfcazshb.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3bcdzyija.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3repxdfwi.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3llyxgyqx.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3rtqysqov.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3wfrijywf.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3qpalilcl.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3vucbvxnn.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3kwesxvof.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3ocxjxucl.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3uprzcnej.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3oijqtevb.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3bydtnlvj.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3koioojvw.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3aqgeonln.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3dpumgjfj.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3zyrlauqi.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3rxghimvb.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3hstrrekt.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3vaaucnyz.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3qxvzdyqa.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3duawzanz.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3oelyqnqn.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3ruyywolv.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3afpjpmaz.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3gsmhdzge.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3pcahyfoz.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3bddejpee.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3lzepctae.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3qxfhzurj.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3atuvxtgd.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3uftnvfvi.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3ygkmmuiv.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3bqtzgwie.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3igvptyju.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3iesyodrd.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3cwveqxod.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3efposhgk.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3uxyfaxcj.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3qcamcarg.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3hmjjfpju.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3ndyglmrv.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3cegqmkxy.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3zftwnglu.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3hniruhat.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3khxusrfc.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3lehsdewo.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3nwoevxij.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3rkjnkwqp.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3neowpxyn.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3xzuxfkfg.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3xaexores.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3btkjpmmz.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3dduqiiri.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3rnmcwphf.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3agkgmncp.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3sydkghry.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3ilefqlcp.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3kfxugmqh.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3lzuculma.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3lgunouka.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3xfyrlnot.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3cqrhjomw.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3fxqhnonl.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3bcvieabq.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3epzslfid.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3gcvawxdj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hamykgrq.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3zpwlwoea.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hliywhoj.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3lipbmanh.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3xnuglxao.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3fpkjzycx.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3prozpjpw.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3ecuqeqmb.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3dcharcxh.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3fkddnfpn.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3vccvjnyj.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3qwtoilxp.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3euouensi.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vdaugpcg.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3tzwrmcsx.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3bcliwmll.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3hswsgwts.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3cvhqvwsp.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3kocbxois.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3zmegccoa.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3umyvmuig.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3qsyuxhdp.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3kqpiopuq.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3eyweakxf.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3bofaxqwr.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3yywaxdea.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3vgzwvuoz.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3fspvgpkg.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3acprnpdf.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3dvzagypp.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3iiurzfbx.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3idcpfkrg.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3zewumccn.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3pffahyzk.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3uphxzmrs.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3mcxjezpu.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3qptfezml.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3rjfhuehw.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3uuvsahtm.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3cdtcpiwd.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3vskadlaz.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3mzrslnrg.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3aohwprnn.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3bpcgptly.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3slluzpkl.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3xkkhdbfk.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3mmvmyqpy.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3tojsbaro.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3asnpmvlx.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3wazsbtjw.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3hklbjxud.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3xhwadsdh.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3fikxdwul.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3zxilbxao.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3yfzqivlv.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3dqygyxof.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3mgktexpn.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3nauobklj.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3hwjiwwlf.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3bvovnypw.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3wleopnak.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3pcwskece.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3ahfoeidl.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3gipamgwg.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3vhvxtwpd.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3dkslajuk.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3oqxzmxkx.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3dduobjlu.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3qupnhsir.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3avlkhzpe.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3anwxduez.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wugrsamb.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3yszpiapp.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3uwtynhwr.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3qasxfper.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3pdxuklpn.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3nlhhfsyn.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3txobtdhj.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3aictsyeq.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3apofujat.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3fcrwfxiu.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3insggvdv.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3frniqogl.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3wfjvzgoi.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3hpjfwlxi.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3mslyesxt.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3dtxckgwf.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3vymvokgt.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3ixxccybu.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3hgwlywdg.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3qizsyhwq.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3bumdqzok.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3mvxkqges.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3fvrrqcjo.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3jtwswivx.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3qbaogedk.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3ctfvvzqo.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3svwbcctf.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3quilzwpo.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3gwqdyofw.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3vmyvchak.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3biyccoxb.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3rrdjnnsw.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3jugppsax.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3daurcngd.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3pztggbba.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3mvegemqa.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3njeqzppe.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3katflkwu.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3rongdknk.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3hzaberdf.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3ccrunzji.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3ugjhonnd.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3kzavcbra.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3idaocyks.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3ucrpopyb.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3qajmprtw.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3bgvumoev.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3qnkdelcs.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3nuxofihz.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3jqvthloj.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3oyygpaay.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3wtpebdwq.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3ijyukpfd.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3iluerkor.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3vvgfvkba.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3eqfcfuja.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3doqtahmx.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3cnjaaavb.html


<!-- 参考信息 -->