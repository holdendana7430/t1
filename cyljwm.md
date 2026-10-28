代发 wailian999

[Q88] 行转列（条件聚合）
来源：http://hz.hammf.cn/gtfwqsliwg.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.pycfn.com/gtauaxrmub.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.pycfn.com/gtzheezpwo.html

[Q89] 判断表是否存在
来源：http://hz.yonumen.top/gtswgictqx.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.hfpthk.cn/gtrsnoejww.html

[Q90] 生成序号列
来源：http://hz.yj20258.top/gtgnkakuzl.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.zhijiandao.cn/gtfkkuwjox.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtcehrmepy.html

R. Bash 专题
来源：http://hz.chenjidiqi.icu/gtruytdivi.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtptdqlvln.html

[R01] shebang 与严格模式
来源：http://hz.xuetiantiany.cn/gtfwrdnabe.html

#!/usr/bin/env bash
来源：http://hz.pengpengdd.cyou/gtumguuobr.html

set -euo pipefail
来源：http://hz.guowangkeji.top/gtcglexfsd.html

[R02] 变量赋值与使用
来源：http://hz.xuetiantiany.cn/gtrfukihbn.html

name="Tom"; echo "$name"
来源：http://hz.shanyushiyangkeji.top/gtkyzqdmix.html

[R03] 只读变量
来源：http://hz.gogol.net.cn/gtlickslsf.html

readonly PI=3.14
来源：http://hz.xinyue.icu/gtarbnmlfb.html

[R04] 位置参数
来源：http://hz.hywenlv.cn/gtwuwbcssp.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.shanyushiyangkeji.top/gtuegvfvrn.html

[R05] 参数默认值
来源：http://hz.ydzc1.top/gtbsjdwgxq.html

name="${1:-default}"
来源：http://hz.shanyushiyangtech.top/gthjppubym.html

[R06] 判断命令是否存在
来源：http://hz.tian-w.cn/gtxezizqzx.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.nanxinkj.top/gtuhqbjzph.html

[R07] if 判断文件
来源：http://hz.xziqi.cn/gtkawulhhp.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.9152youxi.cn/gtmipigrlg.html

[R08] 数值比较
来源：http://hz.zhongyouzk.top/gtgmbmbvut.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.cashguo.top/gtfxyjbnfm.html

[R09] 字符串比较
来源：http://hz.sufxvd.cn/gtnpjkcmwr.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.xylfe.cn/gtliibjimu.html

[R10] 正则匹配
来源：http://hz.pycfn.com/gtymupmbse.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.jinqigufen.top/gtcsszqggj.html

[R11] case 多分支
来源：http://hz.jqgfzy.top/gtpvfptmch.html

case "$1" in
来源：http://hz.hysaishi.cn/gtwsdhqaab.html

start) echo "启动" ;;
来源：http://hz.zhiwuduotai.top/gthrglpbez.html

stop)  echo "停止" ;;
来源：http://hz.haohaochexian.top/gtdfbbedwt.html

*)     echo "未知命令" ;;
来源：http://hz.gaohongyu789.top/gttpebfbzc.html

esac
来源：http://hz.mhx1999.top/gtkilcxseb.html

[R12] for 遍历文件
来源：http://hz.shangyingyoupin.top/gtxadjtgbg.html

for f in *.txt; do echo "$f"; done
来源：http://hz.fengsongda.top/gtzokjhppx.html

[R13] for 计数循环
来源：http://hz.sysykeji.top/gtstrbqzgl.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.dianchejie.cn/gtjuzbrdau.html

[R14] C 风格 for
来源：http://hz.zhaomingkeji.xyz/gttngelfvt.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.xuetiantiany.cn/gtbbobwcwo.html

[R15] while 逐行读文件
来源：http://hz.jlsjyb.cn/gtnnkfrwbo.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.hywenlv.cn/gtvjdsahah.html

[R16] until 等待条件
来源：http://hz.fzhhl.top/gtcmzuginh.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.jiagoushi.top/gtuunlkmgm.html

[R17] 数组定义与取值
来源：http://hz.daxiang520.top/gtxbpbequt.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.wangdashe.top/gtfgafpdtd.html

[R18] 遍历数组
来源：http://hz.yanxiufei.cn/gtubfkrmkw.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.yuxming.cn/gtxzeqadxm.html

[R19] 数组长度
来源：http://hz.jyoumei.cn/gtyzeumahh.html

echo "${#arr[@]}"
来源：http://hz.52xcode.cn/gtzlpeglso.html

[R20] 关联数组（字典）
来源：http://hz.jqgfzy.top/gtzatsbqfy.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.zdqjudy.top/gtufuhlikk.html

[R21] 字符串长度
来源：http://hz.wangshuangyany.cn/gtcfnahfml.html

echo "${#s}"
来源：http://hz.c1oappe.top/gtjviltjen.html

[R22] 截取子串
来源：http://hz.xziqi.cn/gttjsnzlyl.html

echo "${s:0:5}"
来源：http://hz.aibaodan.cn/gtdhcfxued.html

[R23] 字符串替换
来源：http://hz.mhx1999.top/gtjvysutsn.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.birdmap.top/gtynfnajaq.html

[R24] 大小写转换
来源：http://hz.yuxming.cn/gtchsylseu.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.pengpengdd.cyou/gtviwpyctd.html

[R25] 去后缀 / 去前缀
来源：http://hz.shangyingyoupin.top/gtekhszfun.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.yuxming.cn/gtaotkiorq.html

[R26] 命令替换
来源：http://hz.sysykeji.top/gtbusjyovi.html

now=$(date +%F); echo "$now"
来源：http://hz.tian-w.cn/gtrmenbxmw.html

[R27] 算术展开
来源：http://hz.yongpay.top/gtxatbrkzy.html

echo $((1 + 2 * 3))
来源：http://hz.cdnleiting.top/gtcvuygbhh.html

[R28] 浮点运算
来源：http://hz.zhijiandao.cn/gtycdeolhc.html

echo "scale=2; 10/3" | bc
来源：http://hz.xylfe.cn/gtnlinydbn.html

[R29] 定义函数
来源：http://hz.yj20258888.top/gtwqzgsfrn.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.yanxiufei.cn/gtdecbbrte.html

[R30] 函数返回状态码
来源：http://hz.mhx1999.top/gtemtiwbqm.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.0kj1m.cn/gtwpquxtev.html

[R31] 局部变量
来源：http://hz.fzhhl.top/gtwmxabibp.html

f() { local x=1; echo "$x"; }
来源：http://hz.jlsjyb.cn/gtbtkfwdob.html

[R32] 参数个数校验
来源：http://hz.jqgufenzy.top/gtvtyxjavv.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.sxryk.cn/gtitrwnjtx.html

[R33] 捕获错误并提示行号
来源：http://hz.fzhhl.top/gtbrovenuo.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.tanke756.top/gtrkvsyyab.html

[R34] 退出时清理
来源：http://hz.wangshuangyany.cn/gtvokhxnpo.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.chenlongwang.top/gtubpfpvsh.html

[R35] 后台执行并等待
来源：http://hz.yvedp.cn/gtkosxvqhn.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.mhx1999.top/gtsvddgcgh.html

[R36] 并发执行多个任务
来源：http://hz.jinghuilouyu.cn/gtqpjqsibg.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.shzxlz.cn/gtzlwlfklz.html

[R37] 把输出赋给变量
来源：http://hz.chenzaomai.com/gthaikcxky.html

files=$(ls -1)
来源：http://hz.guannengcc.top/gtddoqokgq.html

[R38] 管道串联
来源：http://hz.tanke756.top/gtvgqsmxrh.html

cat a.txt | grep -i error | wc -l
来源：http://hz.havefunace.top/gtsgmboztx.html

[R39] 重定向标准输出与错误
来源：http://hz.yj20258888.top/gtxkgftgjo.html

cmd > out.log 2>&1
来源：http://hz.yueranfly.top/gttyzvbrxf.html

[R40] 追加写日志
来源：http://hz.ivvv.top/gtoibgpvmw.html

echo "log" >> out.log
来源：http://hz.birdmap.top/gtzedwkkcr.html

[R41] 丢弃输出
来源：http://hz.zhiwuduotai.top/gtvybtffys.html

cmd >/dev/null 2>&1
来源：http://hz.hongshengwenyu.top/gtlewcjgjl.html

[R42] 输入重定向
来源：http://hz.snrcjt.cn/gttcjvbtbz.html

wc -l < a.txt
来源：http://hz.xinyue.icu/gtrazanfar.html

[R43] 按名字查找文件
来源：http://hz.zhaomingkeji.xyz/gtfdzxybcm.html

find . -name "*.log" -type f
来源：http://hz.smart0.xyz/gtfjuulwdc.html

[R44] 按修改时间查找
来源：http://hz.yuxming.cn/gtapslegsp.html

find . -mtime -7 -type f
来源：http://hz.aibaodan.cn/gtuahycsem.html

[R45] 批量删除
来源：http://hz.ehwqpu.com/gtvwkokyxb.html

find . -name "*.tmp" -delete
来源：http://hz.zdqjudy.top/gtxfbtaesz.html

[R46] 递归替换文件内容
来源：http://hz.nwbrower.top/gtqwgcjaov.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.chenlongwang.top/gtqjsqqtez.html

[R47] sed 单行替换
来源：http://hz.zycfv.cn/gtedcscmvb.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.guowangkeji.top/gthrfeciyj.html

[R48] awk 取指定列
来源：http://hz.jqgufenzy.top/gtkgjuzpbu.html

awk '{print $1, $3}' a.txt
来源：http://hz.xziqi.cn/gtyjctdsyq.html

[R49] awk 带条件
来源：http://hz.vqdsnc.cn/gtghgkdbuq.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.feifeiyinyue.top/gteqoohngn.html

[R50] awk 求和
来源：http://hz.shuidangran.top/gtkcdedgda.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.shangyingyoupin.top/gtaxnyprjv.html

[R51] 排序去重取前几
来源：http://hz.yj202588.top/gtrrohkodw.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.cheryme.top/gtcosqogpo.html

[R52] 统计行数
来源：http://hz.jlsjyb.cn/gtyhixcoew.html

wc -l a.txt
来源：http://hz.shanyushiyangkeji.top/gteroixaun.html

[R53] 查看文件头与实时尾
来源：http://hz.52xcode.cn/gtflbmzwfn.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.zhoulong.xyz/gtcovgdsir.html

[R54] 比较两个文件
来源：http://hz.xziqi.cn/gtyadafyzj.html

diff a.txt b.txt
来源：http://hz.sysykeji.top/gtgzpwpwld.html

[R55] 压缩与解压
来源：http://hz.tanke756.top/gtnuxupvxi.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.shanyushiyangtech.top/gtxpkapuhf.html

[R56] 远程拷贝
来源：http://hz.quarkkingdee.top/gtkogtudtr.html

scp file user@host:/path/
来源：http://hz.zhengqikj.top/gtkzzagugo.html

[R57] 远程执行命令
来源：http://hz.redwolf501.top/gtiovfswzr.html

ssh user@host 'uptime'
来源：http://hz.xuetiantiany.cn/gtuwcvfcik.html

[R58] 下载文件
来源：http://hz.ydzc1.top/gtclryxehg.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.gzhubu.top/gtmjmsiebk.html

[R59] 发 POST JSON
来源：http://hz.hywenlv.cn/gtrsbclhez.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.chenzaomai.com/gtthbpkopu.html

[R60] 只看 HTTP 状态码
来源：http://hz.yanxiufei.cn/gtmabgbtmi.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.shangyingyoupin.top/gtjsjrbati.html

[R61] 磁盘占用
来源：http://hz.yuxming.cn/gtskboenbw.html

df -h;  du -sh *
来源：http://hz.ydjk.org.cn/gtpsqnxqpu.html

[R62] 找最占空间的文件
来源：http://hz.xingfuxueyuan.xyz/gtvxqbjepd.html

du -ah . | sort -rh | head -10
来源：http://hz.jiagoushi.top/gtqsbfiurb.html

[R63] 内存与进程
来源：http://hz.chenlongwang.top/gtrhwpxegv.html

free -h;  ps aux | grep nginx
来源：http://hz.zhijiandao.cn/gtkzwagovl.html

[R64] 结束进程
来源：http://hz.redwolf501.top/gtxnginnls.html

kill -9 $(pgrep -f app.py)
来源：http://hz.zhengqikj.top/gtkhcgytne.html

[R65] 查看端口占用
来源：http://hz.xylfe.cn/gtyjxsikpa.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.xingfuxueyuan.xyz/gtrmkpjhjf.html

[R66] 定时任务
来源：http://hz.jianghu66.top/gtggtaabbk.html

crontab -e;  crontab -l
来源：http://hz.yj20258888.top/gtdzkswkjc.html

[R67] 生成随机十六进制串
来源：http://hz.cucudq.cn/gtcibsthkd.html

openssl rand -hex 16
来源：http://hz.nanxinkj.top/gtcgviysql.html

[R68] 计算文件校验值
来源：http://hz.hywenlv.cn/gtzlqqdlym.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.yonumen.top/gtdzryqoch.html

[R69] 生成随机密码
来源：http://hz.bjfxy.top/gtmborqnin.html

head -c 16 /dev/urandom | base64
来源：http://hz.yj202588.top/gtwddpmfof.html

[R70] 时间戳与互转
来源：http://hz.havefunace.top/gtgbbvvxbl.html

date +%s;  date -d @1700000000
来源：http://hz.sxryk.cn/gtcwgzvrox.html

[R71] 日期格式化
来源：http://hz.zhiwuduotai.top/gtundosyyf.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.vqdsnc.cn/gtvbbybrxw.html

[R72] 等待端口就绪
来源：http://hz.jinyuanbaomall.cn/gtqbjkzlwz.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.c1oappe.top/gtbiivgbot.html

[R73] 分割大日志
来源：http://hz.guowangkeji.top/gtvhyqbspm.html

split -l 1000 big.log part_
来源：http://hz.tian-w.cn/gtdzssrdss.html

[R74] 批量重命名
来源：http://hz.yuanzhike.top/gtbptyoile.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.jyoumei.cn/gtziqfhudf.html

[R75] 导出环境变量
来源：http://hz.andypj.xyz/gtzocmovxh.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.316326.xyz/gtfhygazbf.html

[R76] 使用临时文件
来源：http://hz.iojbl.cn/gtxlgppgih.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.hywenlv.cn/gtbkmftdjy.html

[R77] 读取用户输入
来源：http://hz.gzhubu.top/gtxrfbvyzd.html

read -rp "请输入: " ans
来源：http://hz.shangyingyoupin.top/gtaqtktzef.html

[R78] 交互式菜单
来源：http://hz.shzxlz.cn/gteyhcipsg.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.yongpay.top/gtszkwgfaa.html

[R79] 解析命令行选项
来源：http://hz.zhijiandao.cn/gtcgbabjmt.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.zhiwuduotai.top/gtdaexsixq.html

[R80] 查看脚本执行耗时
来源：http://hz.bjfxy.top/gtquiomnul.html

time ./run.sh
来源：http://hz.nwbrower.top/gtpqckuxdz.html

================================================================================
来源：http://hz.shzxlz.cn/gtqzzjenpj.html

S. C / C++ 专题
来源：http://hz.feifeiyinyue.top/gtbdzqffzp.html

================================================================================
来源：http://hz.smart0.xyz/gtovfuvgah.html

[S01] C：Hello World
来源：http://hz.haohaochexian.top/gtdylqzamz.html

#include <stdio.h>
来源：http://hz.zhoulong.xyz/gtltaucfhw.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.daxiang520.top/gthqujaymj.html

[S02] C：变量与格式化输出
来源：http://hz.zycfv.cn/gtjutehoba.html

int a = 10; printf("%d\n", a);
来源：http://hz.meibo888.top/gthippului.html

[S03] C：读入整数
来源：http://hz.jiagoushi.top/gtfydinrgr.html

int x; scanf("%d", &x);
来源：http://hz.daxiang520.top/gtylfvjrkc.html

[S04] C：字符串复制
来源：http://hz.sxryk.cn/gtsdwsqpdc.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.aibaodan.cn/gtvmukvomm.html

[S05] C：字符串长度
来源：http://hz.fzhhl.top/gtezlybusa.html

strlen(s)
来源：http://hz.sufxvd.cn/gtnrzzidky.html

[S06] C：字符串比较
来源：http://hz.wangshuangyany.cn/gtdsgkboxo.html

strcmp(a, b) == 0
来源：http://hz.yj20258.top/gtslbufnql.html

[S07] C：数组遍历求和
来源：http://hz.xingfuxueyuan.xyz/gtvsocowlf.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.pycfn.com/gthuzwfade.html

[S08] C：动态内存分配与释放
来源：http://hz.fzhhl.top/gtxglxnujx.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.zhixingplan.top/gtgyscqjqy.html

[S09] C：结构体定义与初始化
来源：http://hz.zhoulong.xyz/gtvuayvsbj.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.yuanzhike.top/gtavobuvro.html

[S10] C：指针与解引用
来源：http://hz.guannengcc.top/gtvaoraakq.html

int *p = &a;  *p = 5;
来源：http://hz.ybcxt.top/gtawmzwekn.html

[S11] C：逐行读文件
来源：http://hz.shanyushiyangkeji.top/gtbytpgwhp.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.fzhhl.top/gttsgeyurf.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.haohaochexian.top/gtqwysbyqu.html

fclose(f);
来源：http://hz.dashuyun.cn/gtoqwcnhyv.html

[S12] C：写文件
来源：http://hz.chenzaomai.com/gtldyiibnx.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.hfpthk.cn/gtohmhbsjz.html

[S13] C：宏定义
来源：http://hz.haohaochexian.top/gtavniculu.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.ydjk.org.cn/gtitabmkln.html

[S14] C：枚举
来源：http://hz.fengsongda.top/gttoovwrdg.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.sufxvd.cn/gtutkuighp.html

[S15] C：类型转换
来源：http://hz.dianchejie.cn/gtnsposkzk.html

(double) a / b
来源：http://hz.zhengqikj.top/gteqsfesgj.html

[S16] C：位操作置位
来源：http://hz.xuetiantiany.cn/gtvmoogdlh.html

x |= (1 << 3);
来源：http://hz.jiagoushi.top/gtczravwbu.html

[S17] C：安全拼接字符串
来源：http://hz.chenjidiqi.icu/gthtlynhon.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.cashguo.top/gtybrjolpq.html

[S18] C：命令行参数
来源：http://hz.svipenyu.cn/gtepilomlr.html

int main(int argc, char **argv)
来源：http://hz.shangyingyoupin.top/gtsbjnpxzc.html

[S19] C：快速排序
来源：http://hz.316326.xyz/gttrbfpstd.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.hongshengwenyu.top/gtltneqbyw.html

[S20] C：二分查找
来源：http://hz.sufxvd.cn/gthxnelkes.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.wangdashe.top/gtjwusuznz.html

[S21] C：字符类别判断
来源：http://hz.yuanzhike.top/gtoifknlqa.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.yangfankeji.com/gtdviebngu.html

[S22] C：字符串转数字
来源：http://hz.andypj.xyz/gtrrriczgh.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.ywan-chungtsiang.top/gtqkrdfgmq.html

[S23] C：随机数
来源：http://hz.havefunace.top/gtjvclqdkm.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.bjfxy.top/gtbfrzeufb.html

[S24] C：获取本地时间
来源：http://hz.yangfankeji.com/gtrlrzgmbb.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.sysykeji.top/gtnzwjzprs.html

[S25] C：内存拷贝
来源：http://hz.snrcjt.cn/gtuqrbegaa.html

memcpy(dst, src, n);
来源：http://hz.yj20258888.top/gtdvngggiv.html

[S26] C：内存清零
来源：http://hz.yonumen.top/gtrqjimplm.html

memset(a, 0, sizeof a);
来源：http://hz.xuanzx.com/gtdtbvnord.html

[S27] C：定义常量
来源：http://hz.zycfv.cn/gttewnmpkm.html

const double PI = 3.14159;
来源：http://hz.nanxinkj.top/gtxvqlsjjq.html

[S28] C：静态变量
来源：http://hz.52xcode.cn/gtobubbvmw.html

static int counter = 0;
来源：http://hz.aizwys.cn/gtoiryfvta.html

[S29] C：变参函数
来源：http://hz.svipenyu.cn/gtsywdjaie.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.ywan-chungtsiang.top/gtxuugrtdu.html

[S30] C：头文件保护
来源：http://hz.svipenyu.cn/gtlbbcibqd.html

#ifndef X_H
来源：http://hz.hongshengwenyu.top/gtguwlwkiv.html

#define X_H
来源：http://hz.yvedp.cn/gthjxpmeqs.html

#endif
来源：http://hz.yuanzhike.top/gtuksjyhsj.html

[S31] C++：Hello World
来源：http://hz.chenlongwang.top/gtogwvhxgx.html

#include <iostream>
来源：http://hz.havefunace.top/gtanozyetz.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.gaohongyu789.top/gtsvxifbjp.html

[S32] C++：字符串
来源：http://hz.ppjwa.cn/gtggejptzz.html

std::string s = "hi";  s += "!";
来源：http://hz.ydzc1.top/gtrjovkaqa.html

[S33] C++：vector 增删
来源：http://hz.guannengcc.top/gtjaqgtuxu.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.jyoumei.cn/gtrxyjicfe.html

[S34] C++：遍历 vector
来源：http://hz.zhengqikj.top/gteppkncsj.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.birdmap.top/gtyqxucckz.html

[S35] C++：map
来源：http://hz.hysaishi.cn/gtjdcgldha.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.bjfxy.top/gtymoovntj.html

[S36] C++：unordered_map
来源：http://hz.hywenlv.cn/gtdctdnrfq.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.52xcode.cn/gtakgwxlmq.html

[S37] C++：set
来源：http://hz.zdqjudy.top/gtufigymop.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.ppjwa.cn/gtfjkravjf.html

[S38] C++：排序
来源：http://hz.xinyue.icu/gtggkosxfw.html

std::sort(v.begin(), v.end());
来源：http://hz.gotoacloud.top/gthhhslbvm.html

[S39] C++：自定义比较器排序
来源：http://hz.zhiwuduotai.top/gtziwuqzqk.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.hywenlv.cn/gtkrzhomxr.html

[S40] C++：查找元素
来源：http://hz.vqdsnc.cn/gtjjeryuih.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.jinqigfzy.top/gtwmwmpump.html

[S41] C++：类与构造函数
来源：http://hz.yongpay.top/gtrejbmfnc.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.xylfe.cn/gtrldppjed.html

[S42] C++：继承与虚函数
来源：http://hz.cashguo.top/gtuvcivork.html

class B : public Base { public: void f() override {} };
来源：http://hz.jinqigufen.top/gtumcgzycx.html

[S43] C++：智能指针
来源：http://hz.mhx1999.top/gtjhbpvnnw.html

auto p = std::make_unique<int>(5);
来源：http://hz.zhongyouzk.top/gtbuemczab.html

[S44] C++：引用传参
来源：http://hz.cashguo.top/gtlwzjcfkl.html

void inc(int &x) { ++x; }
来源：http://hz.nanxuanxn.top/gtpaslplco.html

[S45] C++：lambda
来源：http://hz.zhaomingkeji.xyz/gtfzjgksqt.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.wangshuangyany.cn/gtytfmvhjg.html

[S46] C++：函数模板
来源：http://hz.316326.xyz/gtmdjmupfb.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.tanke756.top/gtvbdtwvwv.html

[S47] C++：结构化绑定遍历
来源：http://hz.jqgfzy.top/gtsnlakrdf.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.jinqigufen.top/gtzbuzkmku.html

[S48] C++：逐行读文件
来源：http://hz.jinqigufen.top/gtfwufveag.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.gogol.net.cn/gtjrshxvts.html

while (std::getline(in, line)) { }
来源：http://hz.aibaodan.cn/gtzqahereq.html

[S49] C++：写文件
来源：http://hz.jinqigfzy.top/gtbnhyqnet.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.cucudq.cn/gtojvyugzm.html

[S50] C++：格式化数字
来源：http://hz.yj20258888.top/gtkcvzasyv.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.cqqwz.cn/gtjtowfsjb.html

[S51] C++：显式类型转换
来源：http://hz.wangshuangyany.cn/gtlctngcgd.html

static_cast<double>(a) / b
来源：http://hz.nwbrower.top/gtlxwitucf.html

[S52] C++：const 与 noexcept
来源：http://hz.wangshuangyany.cn/gtcecghqvy.html

int size() const noexcept { return n_; }
来源：http://hz.zdqjudy.top/gtgnynslss.html

[S53] C++：移动语义
来源：http://hz.yonumen.top/gtxzuipgns.html

std::vector<int> w = std::move(v);
来源：http://hz.nanxinkj.top/gtbdopaddu.html

[S54] C++：异常处理
来源：http://hz.daria6918.cn/gttxjlriqw.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.yueranfly.top/gtkhbjpgui.html

[S55] C++：结构化绑定
来源：http://hz.hysaishi.cn/gtdocsqmdo.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.svipenyu.cn/gtiglzaemj.html

[S56] C++：optional
来源：http://hz.jinqigfzy.top/gtjkwzuqhx.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.tianlin.xyz/gtlxrxaoeu.html

[S57] C++：编译期常量
来源：http://hz.yvedp.cn/gtwjkmshju.html

constexpr int N = 10;
来源：http://hz.nanxinkj.top/gtqghbffjo.html

[S58] C++：命名空间
来源：http://hz.ydzc1.top/gtaywlogdz.html


<!-- 参考信息 -->