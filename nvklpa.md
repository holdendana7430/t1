代发 wailian999

[Q88] 行转列（条件聚合）
来源：http://hz.birdmap.top/gtbfcgmrce.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.cashguo.top/gtywpdmggb.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.snrcjt.cn/gtoopgarxi.html

[Q89] 判断表是否存在
来源：http://hz.cqqwz.cn/gtkgzxzlej.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.yonumen.top/gtlzytimck.html

[Q90] 生成序号列
来源：http://hz.cdnleiting.top/gtbczznohs.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.zhaomingkeji.xyz/gtnksorfxe.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtlggnmnld.html

R. Bash 专题
来源：http://hz.fzhhl.top/gtybyqdlyg.html

================================================================================
来源：http://hz.svipenyu.cn/gtsjjmpdho.html

[R01] shebang 与严格模式
来源：http://hz.ybcxt.top/gtsuksmkhe.html

#!/usr/bin/env bash
来源：http://hz.havefunace.top/gtfdlgbmzq.html

set -euo pipefail
来源：http://hz.hfpthk.cn/gtmkimfiuf.html

[R02] 变量赋值与使用
来源：http://hz.aibaodan.cn/gtgniibqwf.html

name="Tom"; echo "$name"
来源：http://hz.kuanghao11.cn/gtfcrdyant.html

[R03] 只读变量
来源：http://hz.pycfn.com/gtucopwzgg.html

readonly PI=3.14
来源：http://hz.9152youxi.cn/gterpsgzui.html

[R04] 位置参数
来源：http://hz.yanxiufei.cn/gtqyiafyno.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.dianchejie.cn/gtsbmljirl.html

[R05] 参数默认值
来源：http://hz.zhoulong.xyz/gtvjynjsfq.html

name="${1:-default}"
来源：http://hz.tian-w.cn/gtfskqbdei.html

[R06] 判断命令是否存在
来源：http://hz.cheryme.top/gtyqlbmhen.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.jqgfzy.top/gtebcdysjk.html

[R07] if 判断文件
来源：http://hz.sweek.top/gtbimfvesu.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.hongshengwenyu.top/gteliednru.html

[R08] 数值比较
来源：http://hz.ydjk.org.cn/gtbfcubxob.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.yanxiufei.cn/gtnafjxoix.html

[R09] 字符串比较
来源：http://hz.pengpengdd.cyou/gtjobdszji.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.feifeiyinyue.top/gtzchtgbdd.html

[R10] 正则匹配
来源：http://hz.jinghuilouyu.cn/gtthaviark.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.dianchejie.cn/gtrwlgkcbl.html

[R11] case 多分支
来源：http://hz.snrcjt.cn/gtfknrbxez.html

case "$1" in
来源：http://hz.zhongyouzk.top/gtfdkjaohi.html

start) echo "启动" ;;
来源：http://hz.gogol.net.cn/gtcwviyvdd.html

stop)  echo "停止" ;;
来源：http://hz.yj202588.top/gtxklywhgq.html

*)     echo "未知命令" ;;
来源：http://hz.pengpengdd.cyou/gtsofiybqw.html

esac
来源：http://hz.daria6918.cn/gtukgcljmx.html

[R12] for 遍历文件
来源：http://hz.vqdsnc.cn/gtkexlseva.html

for f in *.txt; do echo "$f"; done
来源：http://hz.52xcode.cn/gtjpypmkqk.html

[R13] for 计数循环
来源：http://hz.chenjidiqi.icu/gtiygitziy.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.kuanghao11.cn/gtekvbtgjz.html

[R14] C 风格 for
来源：http://hz.jqgfzy.top/gtieclhfgy.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.andypj.xyz/gtslzprfhy.html

[R15] while 逐行读文件
来源：http://hz.birdmap.top/gtsbzucrvr.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.cucudq.cn/gtecnjarhr.html

[R16] until 等待条件
来源：http://hz.jyoumei.cn/gtdhzhhjhq.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.daria6918.cn/gtpzojxyey.html

[R17] 数组定义与取值
来源：http://hz.cashguo.top/gtfmesimjt.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.feifeiyinyue.top/gtopvqjkds.html

[R18] 遍历数组
来源：http://hz.zhiwuduotai.top/gtcnevfvdz.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.cqqwz.cn/gthvwtyyvr.html

[R19] 数组长度
来源：http://hz.kuanghao11.cn/gtbmoqekud.html

echo "${#arr[@]}"
来源：http://hz.zhixingplan.top/gtkshplrfk.html

[R20] 关联数组（字典）
来源：http://hz.cashguo.top/gtiobmabce.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.tanke756.top/gtldzgtgil.html

[R21] 字符串长度
来源：http://hz.nwbrower.top/gtykmxidff.html

echo "${#s}"
来源：http://hz.ybcxt.top/gttcbbkmtw.html

[R22] 截取子串
来源：http://hz.hywenlv.cn/gtodqihkpd.html

echo "${s:0:5}"
来源：http://hz.yj20258.top/gtkucpqghp.html

[R23] 字符串替换
来源：http://hz.fengsongda.top/gtyxpqoale.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.aibaodan.cn/gthcbecowj.html

[R24] 大小写转换
来源：http://hz.yj20258.top/gtsobtvmzc.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.iojbl.cn/gtxlseywxw.html

[R25] 去后缀 / 去前缀
来源：http://hz.xuanzx.com/gtrshmdzgj.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.fengsongda.top/gtabceslac.html

[R26] 命令替换
来源：http://hz.smart0.xyz/gtgfbllaot.html

now=$(date +%F); echo "$now"
来源：http://hz.hammf.cn/gtrszwuemu.html

[R27] 算术展开
来源：http://hz.yj20258888.top/gtnjfpprjm.html

echo $((1 + 2 * 3))
来源：http://hz.yangfankeji.com/gtqtmhtfmi.html

[R28] 浮点运算
来源：http://hz.xziqi.cn/gtewdmhavr.html

echo "scale=2; 10/3" | bc
来源：http://hz.hfpthk.cn/gtjxiqdunw.html

[R29] 定义函数
来源：http://hz.sufxvd.cn/gtidjiorfh.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.shzxlz.cn/gtpuswaqjs.html

[R30] 函数返回状态码
来源：http://hz.cdnleiting.top/gtgqzhpbaf.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.iojbl.cn/gttwcnvgpp.html

[R31] 局部变量
来源：http://hz.dashuyun.cn/gtbujgdqwj.html

f() { local x=1; echo "$x"; }
来源：http://hz.gaohongyu789.top/gtupfnifcc.html

[R32] 参数个数校验
来源：http://hz.shzxlz.cn/gtyedhdjqy.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.cashguo.top/gtxtlumwed.html

[R33] 捕获错误并提示行号
来源：http://hz.sufxvd.cn/gtxojlihnk.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.shuidangran.top/gtghkktkcw.html

[R34] 退出时清理
来源：http://hz.sweek.top/gtebsbuqun.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.xuanzx.com/gtbfvvcjah.html

[R35] 后台执行并等待
来源：http://hz.chenjidiqi.icu/gtiuzulddw.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.ybcxt.top/gtlxqgyjnd.html

[R36] 并发执行多个任务
来源：http://hz.andypj.xyz/gtqtxkpazy.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.shuidangran.top/gtmdrjfqek.html

[R37] 把输出赋给变量
来源：http://hz.iojbl.cn/gtiyahriim.html

files=$(ls -1)
来源：http://hz.shzxlz.cn/gtyepfihxp.html

[R38] 管道串联
来源：http://hz.jianghu66.top/gtxnuzyfvd.html

cat a.txt | grep -i error | wc -l
来源：http://hz.bjfxy.top/gtnrukqzdb.html

[R39] 重定向标准输出与错误
来源：http://hz.wangshuangyany.cn/gtkgokchme.html

cmd > out.log 2>&1
来源：http://hz.jinqigfzy.top/gttnyxtahb.html

[R40] 追加写日志
来源：http://hz.hfpthk.cn/gtlxqnydxk.html

echo "log" >> out.log
来源：http://hz.feifeiyinyue.top/gtfnsghugn.html

[R41] 丢弃输出
来源：http://hz.shanyushiyangkeji.top/gtiqqjpqvb.html

cmd >/dev/null 2>&1
来源：http://hz.zhiwuduotai.top/gtpxfuhrla.html

[R42] 输入重定向
来源：http://hz.iojbl.cn/gtkdlfoowc.html

wc -l < a.txt
来源：http://hz.redwolf501.top/gtditefncv.html

[R43] 按名字查找文件
来源：http://hz.9152youxi.cn/gtnpffqvbk.html

find . -name "*.log" -type f
来源：http://hz.meibo888.top/gtfxzggcux.html

[R44] 按修改时间查找
来源：http://hz.ybcxt.top/gtypjrhnra.html

find . -mtime -7 -type f
来源：http://hz.hongshengwenyu.top/gtbierzshy.html

[R45] 批量删除
来源：http://hz.gotoacloud.top/gthkigskgq.html

find . -name "*.tmp" -delete
来源：http://hz.shanyushiyangtech.top/gtyispsvgb.html

[R46] 递归替换文件内容
来源：http://hz.jinghuilouyu.cn/gtmgyoxhgv.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.hysaishi.cn/gtvawtinxq.html

[R47] sed 单行替换
来源：http://hz.fzhhl.top/gtkkkdmcex.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.wangshuangyany.cn/gtczqgyumy.html

[R48] awk 取指定列
来源：http://hz.quarkkingdee.top/gtrxcziaya.html

awk '{print $1, $3}' a.txt
来源：http://hz.aizwys.cn/gtaajuqzeo.html

[R49] awk 带条件
来源：http://hz.316326.xyz/gtnhbbgzja.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.9152youxi.cn/gtxtumayyh.html

[R50] awk 求和
来源：http://hz.zhaomingkeji.xyz/gtsojoznpq.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.guannengcc.top/gthauvvvfn.html

[R51] 排序去重取前几
来源：http://hz.hammf.cn/gtmhdjnhdd.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.redwolf501.top/gtsxnuekxq.html

[R52] 统计行数
来源：http://hz.hnqzz.top/gtnwhbfdcb.html

wc -l a.txt
来源：http://hz.yuxming.cn/gtqcyvgbfe.html

[R53] 查看文件头与实时尾
来源：http://hz.yvedp.cn/gtdccpanvv.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.yuxming.cn/gthzfjlpus.html

[R54] 比较两个文件
来源：http://hz.cashguo.top/gtozotsatw.html

diff a.txt b.txt
来源：http://hz.cucudq.cn/gtufsnphee.html

[R55] 压缩与解压
来源：http://hz.yueranfly.top/gtfolytemg.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.havefunace.top/gtrfubnlik.html

[R56] 远程拷贝
来源：http://hz.mhx1999.top/gtlhzlbvhr.html

scp file user@host:/path/
来源：http://hz.tian-w.cn/gtawrgbnlk.html

[R57] 远程执行命令
来源：http://hz.jinghuilouyu.cn/gtoggpxuiq.html

ssh user@host 'uptime'
来源：http://hz.gaohongyu789.top/gtksrdqsvm.html

[R58] 下载文件
来源：http://hz.0kj1m.cn/gtzgcagpme.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.cqqwz.cn/gtotpivruf.html

[R59] 发 POST JSON
来源：http://hz.hywenlv.cn/gtbsahaxzh.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.ydzc1.top/gtthtfvwgu.html

[R60] 只看 HTTP 状态码
来源：http://hz.mhx1999.top/gtatuhmwcc.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.jinqigufen.top/gtpjjswfoc.html

[R61] 磁盘占用
来源：http://hz.xylfe.cn/gtoqczelpq.html

df -h;  du -sh *
来源：http://hz.tian-w.cn/gtvxzqfsyt.html

[R62] 找最占空间的文件
来源：http://hz.tian-w.cn/gtfpidhnkg.html

du -ah . | sort -rh | head -10
来源：http://hz.jlsjyb.cn/gtfzpqnsxu.html

[R63] 内存与进程
来源：http://hz.shanyushiyangtech.top/gtugmjzhhy.html

free -h;  ps aux | grep nginx
来源：http://hz.zdqjudy.top/gtulqrzvfy.html

[R64] 结束进程
来源：http://hz.sxryk.cn/gtcdrkmllh.html

kill -9 $(pgrep -f app.py)
来源：http://hz.gaohongyu789.top/gtpkxkbtac.html

[R65] 查看端口占用
来源：http://hz.shzxlz.cn/gtefenkipr.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.andypj.xyz/gtvqrglizb.html

[R66] 定时任务
来源：http://hz.yj20258.top/gthzthbwnz.html

crontab -e;  crontab -l
来源：http://hz.svipenyu.cn/gtlfszwqnt.html

[R67] 生成随机十六进制串
来源：http://hz.yj20258.top/gtfacmwwcl.html

openssl rand -hex 16
来源：http://hz.ydjk.org.cn/gteaxytaoy.html

[R68] 计算文件校验值
来源：http://hz.yuxming.cn/gtmkponjtw.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.fengsongda.top/gtsxiqfgic.html

[R69] 生成随机密码
来源：http://hz.sufxvd.cn/gtzwlxarln.html

head -c 16 /dev/urandom | base64
来源：http://hz.jiagoushi.top/gtvgaqmzhf.html

[R70] 时间戳与互转
来源：http://hz.guannengcc.top/gtmixqolov.html

date +%s;  date -d @1700000000
来源：http://hz.ywan-chungtsiang.top/gtgspcxsfb.html

[R71] 日期格式化
来源：http://hz.ppjwa.cn/gtoukhqrwb.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.redwolf501.top/gtktnkahnx.html

[R72] 等待端口就绪
来源：http://hz.andypj.xyz/gtzayycdaj.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.0kj1m.cn/gtahewsdzw.html

[R73] 分割大日志
来源：http://hz.316326.xyz/gtuqivunpx.html

split -l 1000 big.log part_
来源：http://hz.fengsongda.top/gtvihkqvln.html

[R74] 批量重命名
来源：http://hz.yj20258888.top/gtorcfpxsr.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.chenzaomai.com/gtoktozywy.html

[R75] 导出环境变量
来源：http://hz.gotoacloud.top/gtsrqbmuzh.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.0kj1m.cn/gtjaqkbcya.html

[R76] 使用临时文件
来源：http://hz.xuetiantiany.cn/gtjagytebo.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.ydjk.org.cn/gtuepzqsuy.html

[R77] 读取用户输入
来源：http://hz.yonumen.top/gtxyxybkks.html

read -rp "请输入: " ans
来源：http://hz.pengpengdd.cyou/gtylakusgp.html

[R78] 交互式菜单
来源：http://hz.wangdashe.top/gtryaigeaf.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.tanke756.top/gtfsvjrcbn.html

[R79] 解析命令行选项
来源：http://hz.jinqigfzy.top/gtlinmujwq.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.yongpay.top/gtuenatnez.html

[R80] 查看脚本执行耗时
来源：http://hz.jqgfzy.top/gtljjcrqxj.html

time ./run.sh
来源：http://hz.shanyushiyangtech.top/gtgeitiwhe.html

================================================================================
来源：http://hz.jinqigfzy.top/gtjntltapp.html

S. C / C++ 专题
来源：http://hz.jianghu66.top/gtakirgdgm.html

================================================================================
来源：http://hz.iojbl.cn/gtdnuqpvzc.html

[S01] C：Hello World
来源：http://hz.yueranfly.top/gtbiaucfrw.html

#include <stdio.h>
来源：http://hz.hnxiangtu.top/gtyoxjzgvf.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.zhijiandao.cn/gtoyunhacn.html

[S02] C：变量与格式化输出
来源：http://hz.ydjk.org.cn/gtrvzpdvun.html

int a = 10; printf("%d\n", a);
来源：http://hz.zdqjudy.top/gtbqatjkjo.html

[S03] C：读入整数
来源：http://hz.aibaodan.cn/gtjrulmwmy.html

int x; scanf("%d", &x);
来源：http://hz.hnxiangtu.top/gttjjqmxmd.html

[S04] C：字符串复制
来源：http://hz.shzxlz.cn/gtvfgxcpeh.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.jinqigufen.top/gtskeiturf.html

[S05] C：字符串长度
来源：http://hz.aizwys.cn/gtuhquzoiu.html

strlen(s)
来源：http://hz.ehwqpu.com/gtehsxjsrq.html

[S06] C：字符串比较
来源：http://hz.feifeiyinyue.top/gtujwckntp.html

strcmp(a, b) == 0
来源：http://hz.jlsjyb.cn/gtccsrytni.html

[S07] C：数组遍历求和
来源：http://hz.haohaochexian.top/gtjtteeiwz.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.0kj1m.cn/gtwtijygwc.html

[S08] C：动态内存分配与释放
来源：http://hz.shangyingyoupin.top/gtjqublyns.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.hnxiangtu.top/gtyjrnkhyz.html

[S09] C：结构体定义与初始化
来源：http://hz.yueranfly.top/gtiruvhgte.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.iojbl.cn/gtoplmhlfx.html

[S10] C：指针与解引用
来源：http://hz.bjfxy.top/gtyyoxxgep.html

int *p = &a;  *p = 5;
来源：http://hz.cqqwz.cn/gtabducghi.html

[S11] C：逐行读文件
来源：http://hz.gogol.net.cn/gtycsqvhoy.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.bjfxy.top/gtdinxppjm.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.0kj1m.cn/gtcgxflsqu.html

fclose(f);
来源：http://hz.gzhubu.top/gtpureodwy.html

[S12] C：写文件
来源：http://hz.yongpay.top/gtojcqunpk.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.ydjk.org.cn/gtdntkxrom.html

[S13] C：宏定义
来源：http://hz.havefunace.top/gtfpdcnnsu.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.yvedp.cn/gtpsffmsrm.html

[S14] C：枚举
来源：http://hz.bjfxy.top/gtuljmlfoc.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.zhongyouzk.top/gtvfrgaojs.html

[S15] C：类型转换
来源：http://hz.nanxuanxn.top/gtbysemcpy.html

(double) a / b
来源：http://hz.snrcjt.cn/gtjyvgoloy.html

[S16] C：位操作置位
来源：http://hz.sysykeji.top/gtiualclsv.html

x |= (1 << 3);
来源：http://hz.xziqi.cn/gtrkdvycto.html

[S17] C：安全拼接字符串
来源：http://hz.andypj.xyz/gteippjebq.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.haohaochexian.top/gtikpaevmw.html

[S18] C：命令行参数
来源：http://hz.shanyushiyangkeji.top/gtiavvfdpu.html

int main(int argc, char **argv)
来源：http://hz.guannengcc.top/gtupmtiaan.html

[S19] C：快速排序
来源：http://hz.jinghuilouyu.cn/gtbcpydcvl.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.svipenyu.cn/gtmezxdzrl.html

[S20] C：二分查找
来源：http://hz.chenlongwang.top/gtzzfyzmgg.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.sufxvd.cn/gtfuwwpbpw.html

[S21] C：字符类别判断
来源：http://hz.andypj.xyz/gtegkpbswz.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.cucudq.cn/gtvlvjxkwx.html

[S22] C：字符串转数字
来源：http://hz.feifeiyinyue.top/gtcemadsma.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.jinghuilouyu.cn/gtpghcpmnh.html

[S23] C：随机数
来源：http://hz.tanke756.top/gtxntyfvag.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.sweek.top/gtyrdvxzhq.html

[S24] C：获取本地时间
来源：http://hz.shangyingyoupin.top/gtkakqfzev.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.jqgufenzy.top/gtsgntcryj.html

[S25] C：内存拷贝
来源：http://hz.yvedp.cn/gtjrgvsktd.html

memcpy(dst, src, n);
来源：http://hz.yonumen.top/gtkxprdfft.html

[S26] C：内存清零
来源：http://hz.xingfuxueyuan.xyz/gthwzbnhwb.html

memset(a, 0, sizeof a);
来源：http://hz.ppjwa.cn/gtjmjwnjmd.html

[S27] C：定义常量
来源：http://hz.shanyushiyangkeji.top/gtouisgkos.html

const double PI = 3.14159;
来源：http://hz.hnqzz.top/gtyrswcuiw.html

[S28] C：静态变量
来源：http://hz.iojbl.cn/gtpyregehc.html

static int counter = 0;
来源：http://hz.yueranfly.top/gtkzedbyln.html

[S29] C：变参函数
来源：http://hz.9152youxi.cn/gtabeudgny.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.yvedp.cn/gtudykaoos.html

[S30] C：头文件保护
来源：http://hz.chenlongwang.top/gtfobwnvmr.html

#ifndef X_H
来源：http://hz.gzhubu.top/gtzkspdbbe.html

#define X_H
来源：http://hz.ywan-chungtsiang.top/gtmlwanycc.html

#endif
来源：http://hz.52xcode.cn/gtsyidtxds.html

[S31] C++：Hello World
来源：http://hz.cheryme.top/gtfesagytx.html

#include <iostream>
来源：http://hz.haohaochexian.top/gtfzvsjihk.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.aibaodan.cn/gtaaxbolzj.html

[S32] C++：字符串
来源：http://hz.yvedp.cn/gtlvvhbhsn.html

std::string s = "hi";  s += "!";
来源：http://hz.zdqjudy.top/gtxstugxsu.html

[S33] C++：vector 增删
来源：http://hz.yuxming.cn/gtbrxddsrn.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.jyoumei.cn/gtddfibnoy.html

[S34] C++：遍历 vector
来源：http://hz.kuanghao11.cn/gtibrgybsw.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.hnxiangtu.top/gtzlgxainb.html

[S35] C++：map
来源：http://hz.gogol.net.cn/gtvvymhvfz.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.nwbrower.top/gtwucdrnsu.html

[S36] C++：unordered_map
来源：http://hz.yonumen.top/gtubptynff.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.52xcode.cn/gtichamsyk.html

[S37] C++：set
来源：http://hz.shanyushiyangkeji.top/gtfnyeiyir.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.gaohongyu789.top/gtuiyqstvv.html

[S38] C++：排序
来源：http://hz.fzhhl.top/gtypfmnori.html

std::sort(v.begin(), v.end());
来源：http://hz.shanyushiyangtech.top/gthcerppdy.html

[S39] C++：自定义比较器排序
来源：http://hz.sysykeji.top/gtdfiyhllv.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.jyoumei.cn/gtapufzsrm.html

[S40] C++：查找元素
来源：http://hz.kuanghao11.cn/gtdmuwuidk.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.andypj.xyz/gtwppjttej.html

[S41] C++：类与构造函数
来源：http://hz.jqgfzy.top/gtxloaqact.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.zycfv.cn/gtntegrpev.html

[S42] C++：继承与虚函数
来源：http://hz.zhengqikj.top/gthhsttzft.html

class B : public Base { public: void f() override {} };
来源：http://hz.yj20258888.top/gtfiycgnlg.html

[S43] C++：智能指针
来源：http://hz.sweek.top/gtwqebunxh.html

auto p = std::make_unique<int>(5);
来源：http://hz.shuidangran.top/gtlveoejtc.html

[S44] C++：引用传参
来源：http://hz.smart0.xyz/gtgjtgcyvw.html

void inc(int &x) { ++x; }
来源：http://hz.nanxuanxn.top/gtgycfvdyl.html

[S45] C++：lambda
来源：http://hz.zhixingplan.top/gtkbvdtqcu.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.yangfankeji.com/gtbxylbsxb.html

[S46] C++：函数模板
来源：http://hz.shanyushiyangkeji.top/gttwltmhde.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.wangshuangyany.cn/gthipcwecs.html

[S47] C++：结构化绑定遍历
来源：http://hz.zdqjudy.top/gtxhbqpcuh.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.shzxlz.cn/gtaouhmjnc.html

[S48] C++：逐行读文件
来源：http://hz.yvedp.cn/gtqjnogjun.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.redwolf501.top/gtgehcyjxj.html

while (std::getline(in, line)) { }
来源：http://hz.316326.xyz/gttcmgoxop.html

[S49] C++：写文件
来源：http://hz.hysaishi.cn/gthluupnpp.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.fzhhl.top/gtmpddeeto.html

[S50] C++：格式化数字
来源：http://hz.c1oappe.top/gtaoeexxam.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.guowangkeji.top/gtsjpevohv.html

[S51] C++：显式类型转换
来源：http://hz.fzhhl.top/gtwclimaku.html

static_cast<double>(a) / b
来源：http://hz.wangshuangyany.cn/gtfpksinse.html

[S52] C++：const 与 noexcept
来源：http://hz.kuanghao11.cn/gteyhcgmrm.html

int size() const noexcept { return n_; }
来源：http://hz.nanxuanxn.top/gtaxusonbf.html

[S53] C++：移动语义
来源：http://hz.xuetiantiany.cn/gtklfqstnu.html

std::vector<int> w = std::move(v);
来源：http://hz.xinyue.icu/gtbkrwdimi.html

[S54] C++：异常处理
来源：http://hz.jiagoushi.top/gtnbdakctx.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.9152youxi.cn/gthkpzqjis.html

[S55] C++：结构化绑定
来源：http://hz.zhongyouzk.top/gtcvysmjgl.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.ehwqpu.com/gtmewrcbvy.html

[S56] C++：optional
来源：http://hz.ehwqpu.com/gtdcewiyjs.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.tian-w.cn/gteonitzpy.html

[S57] C++：编译期常量
来源：http://hz.yuxming.cn/gtwyjjpjuu.html

constexpr int N = 10;
来源：http://hz.zdqjudy.top/gtpsoujtwe.html

[S58] C++：命名空间
来源：http://hz.sweek.top/gteoirzzpt.html


<!-- 参考信息 -->