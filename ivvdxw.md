代发 wailian999

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3zsjfvnyl.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3oglbzymt.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3dnmjrwus.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3sadtflmm.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3qccvqjfr.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3otpeobzv.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3esfdrrig.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3glhkdnjb.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3wvvqslgs.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3frbsmbgx.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3lvcqjslv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3alewvxsk.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3oaddfwfe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xqwgmeed.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3vaheumzg.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3extzgclo.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3dpvcsjyw.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3gsusysai.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3vjnrzcew.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3wsupzldg.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3tevnvyfd.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3xazwpjsv.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3oaqiaqpz.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3qnygzcvy.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3jqxwqihn.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3fifydrwt.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3mvorbnxr.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3dxbotcxt.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3rrlopnkf.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3pbfkclsr.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3lfpedqly.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3mzuoyjnw.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3iezlgsgl.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3mrvrtnzm.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3iclickkk.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3zliywhfc.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3iyzauocv.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3kcrtvotj.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3gzcmvtvi.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3htiuuzwo.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3cmteryvu.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3xzfdyhpl.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3pzjbmhhg.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3nodkabtq.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3vjzpcbyc.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3bevdjnaf.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3mltbwgqf.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3zvzloxyc.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3kkhjufzf.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3tkgbrdzp.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3ajoizwpj.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3rvipusht.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3nnzfiyvc.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3hmxpztzc.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3cfzsznfh.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3rkyrxlzn.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3pwoldbrk.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3gzkwwmve.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3mkwomfqd.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3nzvsqskc.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3ckozltai.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3nowyeadc.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3dwtkrbbn.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3djdsmkpk.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3bnxliahy.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3ypaprizq.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3hybmmlnf.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3tdqoblim.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3kzlqdxqc.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3itsujwos.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3jvdiogzq.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3ngjwvyba.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3wuabivhr.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3aougawoj.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3zizdzmph.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3lxmunkqj.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3xvafkiwy.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3jrybysgz.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3hgjiphvg.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3ybxzbxoe.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pbbvkiwy.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3tmyhkotp.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3amlqijpn.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3ljdsftqk.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3uhgeudtb.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3lffrycpw.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3dgcvrmlo.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3elztjzfh.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3awzrkmme.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3pldynawt.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3ssgqmhox.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3sqwcauvq.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3ndsdjoyc.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3cviisvjx.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3pquwwtjx.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3xiiipxgs.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3wygdysdy.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3eyixkovx.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3sjipxisx.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3twxkhyfr.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3yveejdxo.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3nubwczkz.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3eoknmpkc.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3uhijaccn.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3vdzzcukz.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3kanjntig.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3ilkthyvo.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3vhjoqqay.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3dmrezrnw.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3nsysddmm.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3camoudmd.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3wejbcaay.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3kdigvwxy.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3iexjwtiw.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3suxnlpaq.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3cdvpftix.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3rjtwawuj.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3lfpwuwul.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3phwqgjcq.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3ytkwvpcj.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3hblycpqu.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3txjpjqpo.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3cymlycez.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3lcgoydvq.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3tekppbwk.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3ebwnmuta.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3wbbbyuxw.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3fxmimimt.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3yalxkoin.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3fcdxrqko.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3qjnkbdhk.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3uqtighcg.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3glhicxio.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3papntftg.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3jykyzlji.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3pjvtydwa.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3gagmvsgg.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3rubdrtfg.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3iwisdobf.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3vfssekoz.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3auuotaiu.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3hsukqmkz.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3lrlohgym.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3hfusovek.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3olfytrqy.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3hbkviwed.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3evqoibbr.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3mtwftgpj.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3gmjbxzkr.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3qxtdobnp.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3jcqdxfzi.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3joqllsvs.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3sfohcpiq.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3bgcnmcql.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3lkxuhahl.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3idugtgss.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3gicioujy.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3fdijalpw.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3qvvibxoh.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ekuoypza.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3apfaasrx.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3fusvtvkl.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3alyaivlj.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3ifadyjds.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3airpvesl.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3hogododl.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3lhohdrak.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3uibyymrp.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3scouyhwc.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3eqwziftc.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3soikipoe.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3ourquwpc.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3gqwqbwhl.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3rsjhpdti.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3awncfybf.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3sydxqsxa.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3nvnmphep.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3nhyssqzz.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3cdtqzzwi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yvkcfcym.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3zueofqav.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3htifczqn.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3iflzvrbo.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3plyalane.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3yupchuge.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3mqnbarnz.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3xyzojlso.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3aiulkcph.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3sqvjzkpe.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3lszgwceh.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3otwpkhzs.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3hqosorbh.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3qtjlyfxt.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3ztstocby.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3inkqbtzk.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3ltzhgita.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3jhmbkvhy.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3xzowrguh.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3ywcwktyq.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3bgzfqhxs.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3pzrmmewt.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3xhdumcsp.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3lpdrykqd.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3oyjeyzss.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3cejbrnng.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3qlpdxulz.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3pqboonay.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3oxwdqqnz.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3czfchdvp.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3ekbpkhvf.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3cifzlqhb.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3mogziuvv.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3csvjsqtl.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3tgurdaas.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3yogxtwmy.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3nrtznnyw.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3mowfxeig.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3skwuywzw.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3cvwcabit.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3xdodnysc.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3enhpehgn.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3qkpuqvrw.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3qbhnepaj.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3tyomgmkf.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3pdqmgjcu.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3xdiankcq.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3ehamgrah.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3vtnhjtkc.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3uzorlyiy.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3hfhdpgnp.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3xhhikwvw.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3cjzvbbmz.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3qsqjgahr.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3sncyjenm.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3ppgbkdnc.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3oziunrjp.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3ucnqhzln.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3ubgwozjf.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3qiotzkvr.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3tdjzbkuy.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3oxlpcezu.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3ldgkxqtu.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3thhmosnn.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3opogadhf.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3hjhjmwjx.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3ldgshxzf.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3yewocjfl.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3rfhcxpku.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3parhoyeq.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3cleaoocd.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3lhgpymna.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3brvsquik.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3vjkpbdac.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3folxmfpo.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3nhfjiwle.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3gnjlnlms.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3frfzxhjo.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3utljzmht.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3xpejfjbb.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3vpaipixk.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3vbxxfpbm.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3suapiiyb.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3gkpkjtjj.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3fqefxlcq.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3yhnhyxkr.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3spmkpxfq.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3wzhasudg.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3udsxsuuc.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3xdxykzoe.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3ckrqciri.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3npsplygn.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3aboogcsc.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3cjnraoub.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3ioswtvkq.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3niopmyvi.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3npurhkwa.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3npxgnxmn.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3ozmrorla.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3xyxetcdv.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3omorueti.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ctwzpsnk.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3ffcwocvn.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3vjyowrrh.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3qnleixud.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3bhjpuzmn.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3pqrwnpvs.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3twyhxunt.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3tqqhfcdp.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ytxubzfa.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3zkujtdxk.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3kwoquamp.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3javdxcgi.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3xemoczma.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3aerydvzd.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3hsyoreei.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3ujbpjkqi.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3wvzqvklz.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3akajozxt.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3yontnjlg.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3ncpqyeem.html


<!-- 参考信息 -->