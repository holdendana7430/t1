代发 wailian999

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.gogol.net.cn/gtzhvgegxp.html

[Q90] 生成序号列
来源：http://hz.yongpay.top/gtciighulk.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.zhoulong.xyz/gtiujcquls.html

================================================================================
来源：http://hz.sweek.top/gtbwbpcqyp.html

R. Bash 专题
来源：http://hz.tianlin.xyz/gtspeuvkhh.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtlinxernn.html

[R01] shebang 与严格模式
来源：http://hz.hnxiangtu.top/gtkmnhgnkb.html

#!/usr/bin/env bash
来源：http://hz.meibo888.top/gtcafhsgyw.html

set -euo pipefail
来源：http://hz.chenjidiqi.icu/gtxbvjgcup.html

[R02] 变量赋值与使用
来源：http://hz.tanke756.top/gtltynzcrz.html

name="Tom"; echo "$name"
来源：http://hz.jqgfzy.top/gtfmfaqaqk.html

[R03] 只读变量
来源：http://hz.zhongyouzk.top/gtozddqopw.html

readonly PI=3.14
来源：http://hz.smart0.xyz/gtuzirnhsc.html

[R04] 位置参数
来源：http://hz.cheryme.top/gtamzlphsn.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.yongpay.top/gtjcxxrmsq.html

[R05] 参数默认值
来源：http://hz.yanxiufei.cn/gtuoawewlu.html

name="${1:-default}"
来源：http://hz.ydjk.org.cn/gtxfqvpnvj.html

[R06] 判断命令是否存在
来源：http://hz.ydzc1.top/gtreshqavw.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.wangdashe.top/gtujhqothx.html

[R07] if 判断文件
来源：http://hz.yangfankeji.com/gtfmhlekep.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.jinyuanbaomall.cn/gtmkjuwdrh.html

[R08] 数值比较
来源：http://hz.jiagoushi.top/gtzylozkuw.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.xylfe.cn/gtblvxvoux.html

[R09] 字符串比较
来源：http://hz.pycfn.com/gtmsigmerc.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.feifeiyinyue.top/gtjuwpwliw.html

[R10] 正则匹配
来源：http://hz.jyoumei.cn/gttdrvqetk.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.tian-w.cn/gtmrzqbsfc.html

[R11] case 多分支
来源：http://hz.xylfe.cn/gtspfjjtgz.html

case "$1" in
来源：http://hz.jyoumei.cn/gtwsoioonu.html

start) echo "启动" ;;
来源：http://hz.redwolf501.top/gtcoijsovv.html

stop)  echo "停止" ;;
来源：http://hz.jianghu66.top/gtcscpnygf.html

*)     echo "未知命令" ;;
来源：http://hz.ydzc1.top/gtqlelohto.html

esac
来源：http://hz.jianghu66.top/gttsgfwhgj.html

[R12] for 遍历文件
来源：http://hz.shzxlz.cn/gtdkvyebsf.html

for f in *.txt; do echo "$f"; done
来源：http://hz.yanxiufei.cn/gtxdmrttdc.html

[R13] for 计数循环
来源：http://hz.yangfankeji.com/gtmfqttolj.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.jinqigufen.top/gtfojgepli.html

[R14] C 风格 for
来源：http://hz.gotoacloud.top/gtyccppkij.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.pycfn.com/gtwmvgcixd.html

[R15] while 逐行读文件
来源：http://hz.snrcjt.cn/gtoizfefoj.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.fengsongda.top/gtffvgzgfr.html

[R16] until 等待条件
来源：http://hz.ppjwa.cn/gtfmaytxxi.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.xylfe.cn/gtxdlcigne.html

[R17] 数组定义与取值
来源：http://hz.hywenlv.cn/gtwenmueqy.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.pengpengdd.cyou/gttmvzqufc.html

[R18] 遍历数组
来源：http://hz.aizwys.cn/gtsbhngidn.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.ydjk.org.cn/gtgmuixhad.html

[R19] 数组长度
来源：http://hz.hnxiangtu.top/gtitddbakf.html

echo "${#arr[@]}"
来源：http://hz.vqdsnc.cn/gtctxkwzxq.html

[R20] 关联数组（字典）
来源：http://hz.hongshengwenyu.top/gtptaimvkw.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.vqdsnc.cn/gtasepylci.html

[R21] 字符串长度
来源：http://hz.xuetiantiany.cn/gtvowfcbxq.html

echo "${#s}"
来源：http://hz.9152youxi.cn/gtvndcbnoc.html

[R22] 截取子串
来源：http://hz.ydzc1.top/gtvplldvce.html

echo "${s:0:5}"
来源：http://hz.birdmap.top/gtvqniyovs.html

[R23] 字符串替换
来源：http://hz.pycfn.com/gthljwsdjm.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.shangyingyoupin.top/gtbeqyynes.html

[R24] 大小写转换
来源：http://hz.sufxvd.cn/gtrmcfuzhd.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.yueranfly.top/gtgormgboy.html

[R25] 去后缀 / 去前缀
来源：http://hz.cdnleiting.top/gtielifmfz.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.ybcxt.top/gtcqdnwbdz.html

[R26] 命令替换
来源：http://hz.guannengcc.top/gtbtelxcns.html

now=$(date +%F); echo "$now"
来源：http://hz.zhongyouzk.top/gtlfomgxss.html

[R27] 算术展开
来源：http://hz.mhx1999.top/gtcruklpbe.html

echo $((1 + 2 * 3))
来源：http://hz.jianghu66.top/gtqlfhrkrn.html

[R28] 浮点运算
来源：http://hz.jqgufenzy.top/gtdtlggsoi.html

echo "scale=2; 10/3" | bc
来源：http://hz.zhongyouzk.top/gtazgovgeo.html

[R29] 定义函数
来源：http://hz.shzxlz.cn/gtxxoxbtlj.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.daxiang520.top/gthdgczcid.html

[R30] 函数返回状态码
来源：http://hz.chenzaomai.com/gtbgvanwvq.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.sxryk.cn/gthbctfisa.html

[R31] 局部变量
来源：http://hz.cheryme.top/gtwobgwimz.html

f() { local x=1; echo "$x"; }
来源：http://hz.mhx1999.top/gtrijmwyge.html

[R32] 参数个数校验
来源：http://hz.haohaochexian.top/gtllacprpd.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.jinghuilouyu.cn/gtsdkmlmcq.html

[R33] 捕获错误并提示行号
来源：http://hz.ydzc1.top/gtnsskentc.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.jlsjyb.cn/gtmgjnwutd.html

[R34] 退出时清理
来源：http://hz.vqdsnc.cn/gtyurqvvih.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.zycfv.cn/gteyqsdlxl.html

[R35] 后台执行并等待
来源：http://hz.yangfankeji.com/gtumdoepmb.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.yj202588.top/gtncmlfhic.html

[R36] 并发执行多个任务
来源：http://hz.shuidangran.top/gtiydfuwfo.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.xziqi.cn/gtzcewvicj.html

[R37] 把输出赋给变量
来源：http://hz.sufxvd.cn/gtwiicbrfh.html

files=$(ls -1)
来源：http://hz.cdnleiting.top/gtvaumahdd.html

[R38] 管道串联
来源：http://hz.andypj.xyz/gtgclgrzib.html

cat a.txt | grep -i error | wc -l
来源：http://hz.daxiang520.top/gtckngwxhz.html

[R39] 重定向标准输出与错误
来源：http://hz.shanyushiyangtech.top/gtgrabndeb.html

cmd > out.log 2>&1
来源：http://hz.snrcjt.cn/gtvcvwabcu.html

[R40] 追加写日志
来源：http://hz.52xcode.cn/gtwxhrlvhh.html

echo "log" >> out.log
来源：http://hz.gzhubu.top/gtxyoyiabi.html

[R41] 丢弃输出
来源：http://hz.dashuyun.cn/gtejaljzhr.html

cmd >/dev/null 2>&1
来源：http://hz.tianlin.xyz/gthikxltpd.html

[R42] 输入重定向
来源：http://hz.fengsongda.top/gtdgyfxchs.html

wc -l < a.txt
来源：http://hz.xuanzx.com/gtwacnwceh.html

[R43] 按名字查找文件
来源：http://hz.shzxlz.cn/gtrjqmnysz.html

find . -name "*.log" -type f
来源：http://hz.xylfe.cn/gtxciqkgmp.html

[R44] 按修改时间查找
来源：http://hz.feifeiyinyue.top/gtbppxxiyg.html

find . -mtime -7 -type f
来源：http://hz.hongshengwenyu.top/gtepecgozl.html

[R45] 批量删除
来源：http://hz.zhaomingkeji.xyz/gtzxdmafdp.html

find . -name "*.tmp" -delete
来源：http://hz.mhx1999.top/gtrepvgoel.html

[R46] 递归替换文件内容
来源：http://hz.mhx1999.top/gtvwilfvek.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.shanyushiyangtech.top/gtmihdptcl.html

[R47] sed 单行替换
来源：http://hz.kuanghao11.cn/gtsybggzug.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.kuanghao11.cn/gtpxxiisrz.html

[R48] awk 取指定列
来源：http://hz.hywenlv.cn/gtgyypgyfr.html

awk '{print $1, $3}' a.txt
来源：http://hz.shangyingyoupin.top/gtvyvctapb.html

[R49] awk 带条件
来源：http://hz.jyoumei.cn/gtxuymvqny.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.zhijiandao.cn/gtdoygsgiz.html

[R50] awk 求和
来源：http://hz.jinghuilouyu.cn/gtojbfjcdj.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.guowangkeji.top/gtbhpbcipi.html

[R51] 排序去重取前几
来源：http://hz.zhixingplan.top/gtmdbfrxuj.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.jqgufenzy.top/gtxlpcfshv.html

[R52] 统计行数
来源：http://hz.cashguo.top/gtxzljqzzv.html

wc -l a.txt
来源：http://hz.snrcjt.cn/gtffsalgpt.html

[R53] 查看文件头与实时尾
来源：http://hz.guowangkeji.top/gtunizczje.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.meibo888.top/gtpomyjdeb.html

[R54] 比较两个文件
来源：http://hz.haohaochexian.top/gtpmiysced.html

diff a.txt b.txt
来源：http://hz.yvedp.cn/gtiienvjku.html

[R55] 压缩与解压
来源：http://hz.smart0.xyz/gtudevfpjs.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.vqdsnc.cn/gttyoniigj.html

[R56] 远程拷贝
来源：http://hz.quarkkingdee.top/gtpzbiiahd.html

scp file user@host:/path/
来源：http://hz.jianghu66.top/gtqgqesrqf.html

[R57] 远程执行命令
来源：http://hz.ydzc1.top/gtjryqhzpe.html

ssh user@host 'uptime'
来源：http://hz.smart0.xyz/gtlzlligud.html

[R58] 下载文件
来源：http://hz.yvedp.cn/gtrwcghliq.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.nanxinkj.top/gtyczfwyoh.html

[R59] 发 POST JSON
来源：http://hz.andypj.xyz/gtztszywae.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.gzhubu.top/gtvbouuumw.html

[R60] 只看 HTTP 状态码
来源：http://hz.iojbl.cn/gtobjnvstk.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.ydzc1.top/gtvodnfisd.html

[R61] 磁盘占用
来源：http://hz.jinqigufen.top/gtzonxnosx.html

df -h;  du -sh *
来源：http://hz.svipenyu.cn/gtbxdeahwf.html

[R62] 找最占空间的文件
来源：http://hz.sweek.top/gtuuvfgnqy.html

du -ah . | sort -rh | head -10
来源：http://hz.yueranfly.top/gtfgfbkjpk.html

[R63] 内存与进程
来源：http://hz.cucudq.cn/gtsjlhtpiw.html

free -h;  ps aux | grep nginx
来源：http://hz.yongpay.top/gtaeeownjb.html

[R64] 结束进程
来源：http://hz.gaohongyu789.top/gtpzxuzwqw.html

kill -9 $(pgrep -f app.py)
来源：http://hz.jyoumei.cn/gttoflykbm.html

[R65] 查看端口占用
来源：http://hz.xingfuxueyuan.xyz/gtdqeiqmdl.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.ivvv.top/gtboaqckbz.html

[R66] 定时任务
来源：http://hz.52xcode.cn/gtfpsobbng.html

crontab -e;  crontab -l
来源：http://hz.nanxuanxn.top/gtqdjuuzmf.html

[R67] 生成随机十六进制串
来源：http://hz.cucudq.cn/gthmikjget.html

openssl rand -hex 16
来源：http://hz.jyoumei.cn/gthoqxzsbo.html

[R68] 计算文件校验值
来源：http://hz.daria6918.cn/gtdyynwyvu.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.chenlongwang.top/gtjyqbfecz.html

[R69] 生成随机密码
来源：http://hz.gotoacloud.top/gtbfljaoxu.html

head -c 16 /dev/urandom | base64
来源：http://hz.ywan-chungtsiang.top/gtfsuizokj.html

[R70] 时间戳与互转
来源：http://hz.shangyingyoupin.top/gttivxivbv.html

date +%s;  date -d @1700000000
来源：http://hz.c1oappe.top/gtlpzrtiuz.html

[R71] 日期格式化
来源：http://hz.guannengcc.top/gtbfjdmaor.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.redwolf501.top/gtugiubbmo.html

[R72] 等待端口就绪
来源：http://hz.cheryme.top/gthkmrwxrj.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.ydzc1.top/gtiixoiozh.html

[R73] 分割大日志
来源：http://hz.hammf.cn/gtkmjeibtd.html

split -l 1000 big.log part_
来源：http://hz.andypj.xyz/gtfkiglomr.html

[R74] 批量重命名
来源：http://hz.yonumen.top/gtowjptfqs.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.cdnleiting.top/gtzgboqosj.html

[R75] 导出环境变量
来源：http://hz.hnxiangtu.top/gtxrgwshrr.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.ivvv.top/gtxciyhoct.html

[R76] 使用临时文件
来源：http://hz.wangshuangyany.cn/gtlgdztukh.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.dashuyun.cn/gtvracrija.html

[R77] 读取用户输入
来源：http://hz.zhixingplan.top/gtmjjbnqfd.html

read -rp "请输入: " ans
来源：http://hz.jinqigufen.top/gtoqolfcxp.html

[R78] 交互式菜单
来源：http://hz.chenzaomai.com/gtqbrrpswo.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.0kj1m.cn/gtztpcuhyi.html

[R79] 解析命令行选项
来源：http://hz.hammf.cn/gtumcrouxk.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.hywenlv.cn/gthcmpioee.html

[R80] 查看脚本执行耗时
来源：http://hz.jyoumei.cn/gtbqfagpor.html

time ./run.sh
来源：http://hz.ivvv.top/gtxvebokgm.html

================================================================================
来源：http://hz.fzhhl.top/gtvvwxwxlp.html

S. C / C++ 专题
来源：http://hz.dashuyun.cn/gthumbwxbd.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtjpatshli.html

[S01] C：Hello World
来源：http://hz.jinqigufen.top/gtzhtffswg.html

#include <stdio.h>
来源：http://hz.jianghu66.top/gthdvaeofc.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.yuxming.cn/gtiscacmal.html

[S02] C：变量与格式化输出
来源：http://hz.zhoulong.xyz/gtspyhdfan.html

int a = 10; printf("%d\n", a);
来源：http://hz.zhixingplan.top/gtjvwpezfw.html

[S03] C：读入整数
来源：http://hz.chenjidiqi.icu/gttdvrrnyo.html

int x; scanf("%d", &x);
来源：http://hz.havefunace.top/gtdsytgyvt.html

[S04] C：字符串复制
来源：http://hz.yueranfly.top/gtlrawinfn.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.52xcode.cn/gtbsqkpxul.html

[S05] C：字符串长度
来源：http://hz.feifeiyinyue.top/gtbhtxlgct.html

strlen(s)
来源：http://hz.zhiwuduotai.top/gtkaeumtpt.html

[S06] C：字符串比较
来源：http://hz.jqgufenzy.top/gtfplzwgkb.html

strcmp(a, b) == 0
来源：http://hz.jinghuilouyu.cn/gtterjdiyk.html

[S07] C：数组遍历求和
来源：http://hz.gzhubu.top/gtbbcfwtwe.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.tanke756.top/gthsnjkmlc.html

[S08] C：动态内存分配与释放
来源：http://hz.nanxuanxn.top/gtrwxtwhmk.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.nanxuanxn.top/gtltroumcm.html

[S09] C：结构体定义与初始化
来源：http://hz.tian-w.cn/gtbqlcdocc.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.birdmap.top/gtgueahavt.html

[S10] C：指针与解引用
来源：http://hz.hnqzz.top/gtydluarhq.html

int *p = &a;  *p = 5;
来源：http://hz.iojbl.cn/gthcysnvcb.html

[S11] C：逐行读文件
来源：http://hz.ppjwa.cn/gtwojovccp.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.zhijiandao.cn/gtvxfcfcsp.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.fengsongda.top/gtlhpvmvgv.html

fclose(f);
来源：http://hz.yuxming.cn/gthhjpyzhv.html

[S12] C：写文件
来源：http://hz.xuanzx.com/gtdaxhdhab.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.sweek.top/gtwporycaa.html

[S13] C：宏定义
来源：http://hz.yangfankeji.com/gtiisiypdf.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.daxiang520.top/gtgrhxfzjy.html

[S14] C：枚举
来源：http://hz.xuanzx.com/gtaxfiokrm.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.aizwys.cn/gtpdhcgiby.html

[S15] C：类型转换
来源：http://hz.havefunace.top/gtvtirwopy.html

(double) a / b
来源：http://hz.iojbl.cn/gtkinoogam.html

[S16] C：位操作置位
来源：http://hz.nanxuanxn.top/gtrccrbmvs.html

x |= (1 << 3);
来源：http://hz.fzhhl.top/gtrtzwmjrk.html

[S17] C：安全拼接字符串
来源：http://hz.pengpengdd.cyou/gteskaxzgy.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.daria6918.cn/gtmckffqih.html

[S18] C：命令行参数
来源：http://hz.dianchejie.cn/gtienecoyx.html

int main(int argc, char **argv)
来源：http://hz.shzxlz.cn/gtoxxvmftp.html

[S19] C：快速排序
来源：http://hz.tian-w.cn/gtdvojizmy.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.52xcode.cn/gtrsnnttpj.html

[S20] C：二分查找
来源：http://hz.ydjk.org.cn/gtdnekeeon.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.xuetiantiany.cn/gtwycdpaax.html

[S21] C：字符类别判断
来源：http://hz.shangyingyoupin.top/gtavwqskzc.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.jqgufenzy.top/gtlzgcbwuh.html

[S22] C：字符串转数字
来源：http://hz.xingfuxueyuan.xyz/gtltssiqwc.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.shanyushiyangkeji.top/gtaqjedjzo.html

[S23] C：随机数
来源：http://hz.pengpengdd.cyou/gtetsmoxhm.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.xuanzx.com/gtomqwxrhc.html

[S24] C：获取本地时间
来源：http://hz.jqgfzy.top/gtlxgoqnpq.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.jqgufenzy.top/gtcetrmfto.html

[S25] C：内存拷贝
来源：http://hz.pycfn.com/gtadsjxqtr.html

memcpy(dst, src, n);
来源：http://hz.bjfxy.top/gtlgebhzer.html

[S26] C：内存清零
来源：http://hz.jqgfzy.top/gtfeznncbf.html

memset(a, 0, sizeof a);
来源：http://hz.zhijiandao.cn/gttnptlxyv.html

[S27] C：定义常量
来源：http://hz.yueranfly.top/gttbypsevk.html

const double PI = 3.14159;
来源：http://hz.0kj1m.cn/gtowautxjz.html

[S28] C：静态变量
来源：http://hz.haohaochexian.top/gtbjqxqako.html

static int counter = 0;
来源：http://hz.shanyushiyangkeji.top/gtgernqapq.html

[S29] C：变参函数
来源：http://hz.sysykeji.top/gtvvwdhmai.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.dianchejie.cn/gthgajbobh.html

[S30] C：头文件保护
来源：http://hz.cashguo.top/gtfeqtpqbu.html

#ifndef X_H
来源：http://hz.shanyushiyangtech.top/gtyqquouzc.html

#define X_H
来源：http://hz.nwbrower.top/gtqloqqsbg.html

#endif
来源：http://hz.pengpengdd.cyou/gtiwjwbjam.html

[S31] C++：Hello World
来源：http://hz.pengpengdd.cyou/gtfaljlhcu.html

#include <iostream>
来源：http://hz.wangshuangyany.cn/gtpldgkmfz.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.ppjwa.cn/gtaymmxgwd.html

[S32] C++：字符串
来源：http://hz.xingfuxueyuan.xyz/gtqjrdyugj.html

std::string s = "hi";  s += "!";
来源：http://hz.hfpthk.cn/gtlpkbkttz.html

[S33] C++：vector 增删
来源：http://hz.cashguo.top/gtmzzddwsv.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.gogol.net.cn/gtcxrwnjmh.html

[S34] C++：遍历 vector
来源：http://hz.52xcode.cn/gtmimrrpqr.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.chenjidiqi.icu/gtlgzkysfy.html

[S35] C++：map
来源：http://hz.bjfxy.top/gtizjrpxit.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.zhoulong.xyz/gtzomjoubt.html

[S36] C++：unordered_map
来源：http://hz.shzxlz.cn/gttekyqlbn.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.sweek.top/gtqpjbegpa.html

[S37] C++：set
来源：http://hz.daxiang520.top/gtnpljlxig.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.xinyue.icu/gtsowiwfhs.html

[S38] C++：排序
来源：http://hz.sufxvd.cn/gtkwdftlcp.html

std::sort(v.begin(), v.end());
来源：http://hz.aizwys.cn/gtwaacmpmh.html

[S39] C++：自定义比较器排序
来源：http://hz.birdmap.top/gtlqqfzlcz.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.chenlongwang.top/gtvilzfjwm.html

[S40] C++：查找元素
来源：http://hz.daxiang520.top/gtjwbzzcdh.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.shuidangran.top/gtlvxxqqzj.html

[S41] C++：类与构造函数
来源：http://hz.jinghuilouyu.cn/gtyeqmrina.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.jinqigfzy.top/gtsziqjlhz.html

[S42] C++：继承与虚函数
来源：http://hz.xinyue.icu/gtdpapzpjy.html

class B : public Base { public: void f() override {} };
来源：http://hz.andypj.xyz/gtppfwfuvm.html

[S43] C++：智能指针
来源：http://hz.snrcjt.cn/gtgckgselp.html

auto p = std::make_unique<int>(5);
来源：http://hz.havefunace.top/gtadbczilt.html

[S44] C++：引用传参
来源：http://hz.shuidangran.top/gtoskxeqlj.html

void inc(int &x) { ++x; }
来源：http://hz.feifeiyinyue.top/gtsiwcrvbm.html

[S45] C++：lambda
来源：http://hz.jinqigufen.top/gtsdipnelj.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.hysaishi.cn/gtgcanqvxw.html

[S46] C++：函数模板
来源：http://hz.svipenyu.cn/gtmljdsjqd.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.sysykeji.top/gtxrxxgqem.html

[S47] C++：结构化绑定遍历
来源：http://hz.feifeiyinyue.top/gtjmlouaqk.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.yangfankeji.com/gtzrjmnjyd.html

[S48] C++：逐行读文件
来源：http://hz.svipenyu.cn/gtrxuztpey.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.hongshengwenyu.top/gtmrhungix.html

while (std::getline(in, line)) { }
来源：http://hz.zhijiandao.cn/gtftnusymz.html

[S49] C++：写文件
来源：http://hz.mhx1999.top/gtnhuinkar.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.9152youxi.cn/gttbcptiev.html

[S50] C++：格式化数字
来源：http://hz.zhaomingkeji.xyz/gtypnucsau.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.zhongyouzk.top/gtlwrtaqxc.html

[S51] C++：显式类型转换
来源：http://hz.vqdsnc.cn/gtbfxthzve.html

static_cast<double>(a) / b
来源：http://hz.bjfxy.top/gtbgluygmx.html

[S52] C++：const 与 noexcept
来源：http://hz.yuxming.cn/gtliydostz.html

int size() const noexcept { return n_; }
来源：http://hz.jiagoushi.top/gturipfsqn.html

[S53] C++：移动语义
来源：http://hz.smart0.xyz/gtxbvkmpbd.html

std::vector<int> w = std::move(v);
来源：http://hz.nanxuanxn.top/gtkrouqzme.html

[S54] C++：异常处理
来源：http://hz.nanxuanxn.top/gtjzknblhs.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.zhiwuduotai.top/gtrlsyrjfb.html

[S55] C++：结构化绑定
来源：http://hz.mhx1999.top/gtrpecihuj.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.nanxuanxn.top/gtwxghqsfx.html

[S56] C++：optional
来源：http://hz.yanxiufei.cn/gtdzwnxrfi.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.jianghu66.top/gtiajwdroc.html

[S57] C++：编译期常量
来源：http://hz.shanyushiyangkeji.top/gtusxezsxl.html

constexpr int N = 10;
来源：http://hz.xinyue.icu/gtakxmdmvk.html

[S58] C++：命名空间
来源：http://hz.cheryme.top/gtgdupubzq.html

namespace ns { int f() { return 1; } }
来源：http://hz.cdnleiting.top/gtycplqsys.html

[S59] C++：静态断言
来源：http://hz.nanxuanxn.top/gtqgltolkn.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.pengpengdd.cyou/gtthnxijxs.html

[S60] C++：遍历并删除元素
来源：http://hz.guowangkeji.top/gtqaysvqwd.html


<!-- 参考信息 -->