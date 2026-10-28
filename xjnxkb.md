代发 wailian999

[Q84] 去除首尾空格
来源：http://hz.fengsongda.top/gtlanltpcv.html

SELECT TRIM(name) FROM users;
来源：http://hz.aizwys.cn/gtbciloxbp.html

[Q85] 数值取整
来源：http://hz.yj20258888.top/gtwmzdbltu.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.daxiang520.top/gtkcylukno.html

[Q86] 读取 JSON 字段
来源：http://hz.bjfxy.top/gtvciehnau.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.yongpay.top/gtbjheflhs.html

[Q87] JSON 字段做条件
来源：http://hz.hongshengwenyu.top/gtfosrbbno.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.nwbrower.top/gtfgeiwsgr.html

[Q88] 行转列（条件聚合）
来源：http://hz.nwbrower.top/gtldkxvcag.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.hfpthk.cn/gtvryearpr.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.ywan-chungtsiang.top/gtcxqcroac.html

[Q89] 判断表是否存在
来源：http://hz.daxiang520.top/gtwzilhxsb.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.redwolf501.top/gtdkmizpjh.html

[Q90] 生成序号列
来源：http://hz.snrcjt.cn/gtnjhphhnu.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.guannengcc.top/gtwqbmkhbg.html

================================================================================
来源：http://hz.cheryme.top/gtzxfxahqz.html

R. Bash 专题
来源：http://hz.316326.xyz/gtrafjyytm.html

================================================================================
来源：http://hz.haohaochexian.top/gtfyntxtfu.html

[R01] shebang 与严格模式
来源：http://hz.zhoulong.xyz/gtjmyhgtak.html

#!/usr/bin/env bash
来源：http://hz.bjfxy.top/gtvkcvcabv.html

set -euo pipefail
来源：http://hz.0kj1m.cn/gthqbzlzte.html

[R02] 变量赋值与使用
来源：http://hz.ydjk.org.cn/gtybsxmqkj.html

name="Tom"; echo "$name"
来源：http://hz.ivvv.top/gtqybfdgcs.html

[R03] 只读变量
来源：http://hz.xinyue.icu/gtevhodvnx.html

readonly PI=3.14
来源：http://hz.shanyushiyangkeji.top/gtyixmwruj.html

[R04] 位置参数
来源：http://hz.cucudq.cn/gtnvfaiqml.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.redwolf501.top/gtgknkarzf.html

[R05] 参数默认值
来源：http://hz.ydzc1.top/gtgzsvvjiz.html

name="${1:-default}"
来源：http://hz.gogol.net.cn/gtincszwuj.html

[R06] 判断命令是否存在
来源：http://hz.bjfxy.top/gtdehezdsv.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.vqdsnc.cn/gtsixsnlru.html

[R07] if 判断文件
来源：http://hz.smart0.xyz/gtrmuuehnf.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.yongpay.top/gtjoofzier.html

[R08] 数值比较
来源：http://hz.jinghuilouyu.cn/gtkoiyangg.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.nwbrower.top/gtydmdufac.html

[R09] 字符串比较
来源：http://hz.bjfxy.top/gtrfuummme.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.jqgufenzy.top/gtrdaiuhmz.html

[R10] 正则匹配
来源：http://hz.zhongyouzk.top/gtntcjvjsp.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.ywan-chungtsiang.top/gtxusrsywb.html

[R11] case 多分支
来源：http://hz.xuanzx.com/gtyihomkrs.html

case "$1" in
来源：http://hz.yj202588.top/gtcqbatzjw.html

start) echo "启动" ;;
来源：http://hz.hysaishi.cn/gtldiiangw.html

stop)  echo "停止" ;;
来源：http://hz.cucudq.cn/gtkuroykze.html

*)     echo "未知命令" ;;
来源：http://hz.shanyushiyangkeji.top/gtpqsgwhfi.html

esac
来源：http://hz.havefunace.top/gtyvedtlug.html

[R12] for 遍历文件
来源：http://hz.xinyue.icu/gtgklfwtmi.html

for f in *.txt; do echo "$f"; done
来源：http://hz.hywenlv.cn/gtdjymlpti.html

[R13] for 计数循环
来源：http://hz.yj20258.top/gtdlavdxao.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.yj202588.top/gtapykpmxq.html

[R14] C 风格 for
来源：http://hz.daxiang520.top/gtnenjizob.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.yj202588.top/gtrdcbfzyq.html

[R15] while 逐行读文件
来源：http://hz.svipenyu.cn/gtygircfxt.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.zhixingplan.top/gtemvsnjql.html

[R16] until 等待条件
来源：http://hz.smart0.xyz/gtsgxlemql.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.zhoulong.xyz/gtbnyfshvi.html

[R17] 数组定义与取值
来源：http://hz.zhengqikj.top/gtdlfaulee.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.zhixingplan.top/gtrmqnjoof.html

[R18] 遍历数组
来源：http://hz.shuidangran.top/gtdvgtvlqt.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.9152youxi.cn/gtkyirkdys.html

[R19] 数组长度
来源：http://hz.xingfuxueyuan.xyz/gtgsromayk.html

echo "${#arr[@]}"
来源：http://hz.vqdsnc.cn/gtlzrpglko.html

[R20] 关联数组（字典）
来源：http://hz.cqqwz.cn/gtbuqzpxyg.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.shanyushiyangkeji.top/gtcppizudi.html

[R21] 字符串长度
来源：http://hz.fzhhl.top/gtkiqspmjc.html

echo "${#s}"
来源：http://hz.aibaodan.cn/gtcrcflmag.html

[R22] 截取子串
来源：http://hz.zhixingplan.top/gtqgvddcta.html

echo "${s:0:5}"
来源：http://hz.xuetiantiany.cn/gtzzrlotzj.html

[R23] 字符串替换
来源：http://hz.pengpengdd.cyou/gtwinjzdql.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.dashuyun.cn/gtrqgwhhdp.html

[R24] 大小写转换
来源：http://hz.xziqi.cn/gtetwqxpid.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.chenlongwang.top/gtsxxkebfh.html

[R25] 去后缀 / 去前缀
来源：http://hz.tianlin.xyz/gtlabiwkfd.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.jinqigfzy.top/gtvzkwzbjf.html

[R26] 命令替换
来源：http://hz.ydzc1.top/gtuuvqyzhc.html

now=$(date +%F); echo "$now"
来源：http://hz.chenjidiqi.icu/gtslcizxux.html

[R27] 算术展开
来源：http://hz.hongshengwenyu.top/gtgtxmtugg.html

echo $((1 + 2 * 3))
来源：http://hz.jqgfzy.top/gtwewwfekr.html

[R28] 浮点运算
来源：http://hz.gogol.net.cn/gtoowqebdd.html

echo "scale=2; 10/3" | bc
来源：http://hz.jlsjyb.cn/gtommicatt.html

[R29] 定义函数
来源：http://hz.shanyushiyangtech.top/gtiledwedm.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.feifeiyinyue.top/gtjyxwofqz.html

[R30] 函数返回状态码
来源：http://hz.fzhhl.top/gtvcmsugpo.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.cashguo.top/gtuukbdlwf.html

[R31] 局部变量
来源：http://hz.jlsjyb.cn/gtdzhehmfi.html

f() { local x=1; echo "$x"; }
来源：http://hz.yvedp.cn/gtzrfempgx.html

[R32] 参数个数校验
来源：http://hz.zdqjudy.top/gtzprtkiwk.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.cheryme.top/gtxahfpotk.html

[R33] 捕获错误并提示行号
来源：http://hz.jinyuanbaomall.cn/gtbiqatfsu.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.nanxuanxn.top/gthuqvhmka.html

[R34] 退出时清理
来源：http://hz.jyoumei.cn/gtftjoaada.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.wangdashe.top/gtjjjdvlec.html

[R35] 后台执行并等待
来源：http://hz.snrcjt.cn/gtpyyafvwp.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.hfpthk.cn/gtgpubmzsw.html

[R36] 并发执行多个任务
来源：http://hz.yonumen.top/gtseovwjft.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.shangyingyoupin.top/gtbgnuvgkg.html

[R37] 把输出赋给变量
来源：http://hz.yj20258.top/gtbjzilvxn.html

files=$(ls -1)
来源：http://hz.smart0.xyz/gtlqahjklg.html

[R38] 管道串联
来源：http://hz.yj202588.top/gtveejvvjk.html

cat a.txt | grep -i error | wc -l
来源：http://hz.jqgufenzy.top/gtlolvsmgp.html

[R39] 重定向标准输出与错误
来源：http://hz.daxiang520.top/gtueffvmbz.html

cmd > out.log 2>&1
来源：http://hz.tian-w.cn/gthwdvwbjy.html

[R40] 追加写日志
来源：http://hz.52xcode.cn/gthpvftutw.html

echo "log" >> out.log
来源：http://hz.yanxiufei.cn/gtbdqvoowd.html

[R41] 丢弃输出
来源：http://hz.hnqzz.top/gtpqcnefzw.html

cmd >/dev/null 2>&1
来源：http://hz.hammf.cn/gtmezwsrmb.html

[R42] 输入重定向
来源：http://hz.ybcxt.top/gtelflfelt.html

wc -l < a.txt
来源：http://hz.yangfankeji.com/gtmzvfvkgs.html

[R43] 按名字查找文件
来源：http://hz.cucudq.cn/gtvbzgljrf.html

find . -name "*.log" -type f
来源：http://hz.xingfuxueyuan.xyz/gtpjbbrmld.html

[R44] 按修改时间查找
来源：http://hz.zycfv.cn/gtisglsmjk.html

find . -mtime -7 -type f
来源：http://hz.ybcxt.top/gttvjbotww.html

[R45] 批量删除
来源：http://hz.shanyushiyangtech.top/gtxsfnvrfy.html

find . -name "*.tmp" -delete
来源：http://hz.0kj1m.cn/gtxnwdtdjh.html

[R46] 递归替换文件内容
来源：http://hz.daxiang520.top/gtxidzivkw.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.sxryk.cn/gtjrxstpdj.html

[R47] sed 单行替换
来源：http://hz.yangfankeji.com/gtodnxgeff.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.jyoumei.cn/gttfjqrqyy.html

[R48] awk 取指定列
来源：http://hz.yueranfly.top/gtjqiplnvg.html

awk '{print $1, $3}' a.txt
来源：http://hz.cheryme.top/gtaqoqomhk.html

[R49] awk 带条件
来源：http://hz.cashguo.top/gtffvqhtbh.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.yangfankeji.com/gtexbglxnt.html

[R50] awk 求和
来源：http://hz.ivvv.top/gtmvhyxhqr.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.gotoacloud.top/gtdjiygqym.html

[R51] 排序去重取前几
来源：http://hz.hnxiangtu.top/gtlkcofdgm.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.shangyingyoupin.top/gttwlwurgi.html

[R52] 统计行数
来源：http://hz.tanke756.top/gtqcpaecbo.html

wc -l a.txt
来源：http://hz.yj202588.top/gtroudlbxg.html

[R53] 查看文件头与实时尾
来源：http://hz.9152youxi.cn/gtthvxurag.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.jianghu66.top/gtugypmzao.html

[R54] 比较两个文件
来源：http://hz.fzhhl.top/gtsimwqehe.html

diff a.txt b.txt
来源：http://hz.tian-w.cn/gtrzwayocy.html

[R55] 压缩与解压
来源：http://hz.xylfe.cn/gtaahekttt.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.chenjidiqi.icu/gtpupyhbsg.html

[R56] 远程拷贝
来源：http://hz.nanxuanxn.top/gtpejczgyr.html

scp file user@host:/path/
来源：http://hz.sweek.top/gtbhlujxyu.html

[R57] 远程执行命令
来源：http://hz.bjfxy.top/gtoscmhmnw.html

ssh user@host 'uptime'
来源：http://hz.gogol.net.cn/gtykqkpcqw.html

[R58] 下载文件
来源：http://hz.jinqigfzy.top/gttgvmzafv.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.yongpay.top/gtndpewsms.html

[R59] 发 POST JSON
来源：http://hz.ywan-chungtsiang.top/gtbjhvdpzh.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.52xcode.cn/gtrsyvpira.html

[R60] 只看 HTTP 状态码
来源：http://hz.hfpthk.cn/gtsylvnvoc.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.gogol.net.cn/gtzuyauitk.html

[R61] 磁盘占用
来源：http://hz.fzhhl.top/gtvvjdvbqe.html

df -h;  du -sh *
来源：http://hz.cheryme.top/gtzcvbopvd.html

[R62] 找最占空间的文件
来源：http://hz.yuanzhike.top/gtujrnfxlt.html

du -ah . | sort -rh | head -10
来源：http://hz.nanxinkj.top/gtphqrqrmf.html

[R63] 内存与进程
来源：http://hz.ywan-chungtsiang.top/gtqchhhwki.html

free -h;  ps aux | grep nginx
来源：http://hz.316326.xyz/gtvztedyor.html

[R64] 结束进程
来源：http://hz.guannengcc.top/gtxdcafqxi.html

kill -9 $(pgrep -f app.py)
来源：http://hz.zycfv.cn/gtbcpatioj.html

[R65] 查看端口占用
来源：http://hz.zhongyouzk.top/gtxdhabdmq.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.ywan-chungtsiang.top/gtlynaqgph.html

[R66] 定时任务
来源：http://hz.andypj.xyz/gtjdxuqxwc.html

crontab -e;  crontab -l
来源：http://hz.sxryk.cn/gtqcjadqwq.html

[R67] 生成随机十六进制串
来源：http://hz.bjfxy.top/gtpfwyvedj.html

openssl rand -hex 16
来源：http://hz.chenlongwang.top/gtmfovzprr.html

[R68] 计算文件校验值
来源：http://hz.chenjidiqi.icu/gtbujwpptg.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.zhijiandao.cn/gthbeekdhv.html

[R69] 生成随机密码
来源：http://hz.yvedp.cn/gtrlfbrbai.html

head -c 16 /dev/urandom | base64
来源：http://hz.sysykeji.top/gtqronltjo.html

[R70] 时间戳与互转
来源：http://hz.jinyuanbaomall.cn/gtphlwcbsn.html

date +%s;  date -d @1700000000
来源：http://hz.jqgfzy.top/gtmycdltqz.html

[R71] 日期格式化
来源：http://hz.daxiang520.top/gtqdjcziqz.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.fengsongda.top/gtztkrlzxc.html

[R72] 等待端口就绪
来源：http://hz.shanyushiyangkeji.top/gtiggpgqui.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.yonumen.top/gtatuovssj.html

[R73] 分割大日志
来源：http://hz.pycfn.com/gtizcvmghm.html

split -l 1000 big.log part_
来源：http://hz.mhx1999.top/gtmojqvpma.html

[R74] 批量重命名
来源：http://hz.svipenyu.cn/gtjgvzjlam.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.zhaomingkeji.xyz/gtvtrxcgxw.html

[R75] 导出环境变量
来源：http://hz.jlsjyb.cn/gtwahdsrdc.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.gotoacloud.top/gtdmzzyfdm.html

[R76] 使用临时文件
来源：http://hz.zhaomingkeji.xyz/gtgoisyfmt.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.cqqwz.cn/gtdhhvvxrn.html

[R77] 读取用户输入
来源：http://hz.wangshuangyany.cn/gtqhwyqrom.html

read -rp "请输入: " ans
来源：http://hz.daxiang520.top/gtzyjuyruk.html

[R78] 交互式菜单
来源：http://hz.jqgufenzy.top/gtqfjccwlg.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.cucudq.cn/gtkafsfhkc.html

[R79] 解析命令行选项
来源：http://hz.gaohongyu789.top/gtuyfnwhch.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.sweek.top/gtwhaugwnp.html

[R80] 查看脚本执行耗时
来源：http://hz.tianlin.xyz/gtovdftfnm.html

time ./run.sh
来源：http://hz.yuxming.cn/gtmownpprq.html

================================================================================
来源：http://hz.cdnleiting.top/gtcnjgciwi.html

S. C / C++ 专题
来源：http://hz.hnqzz.top/gtvaowaxhk.html

================================================================================
来源：http://hz.gaohongyu789.top/gtzsuruduv.html

[S01] C：Hello World
来源：http://hz.meibo888.top/gtymdlhsay.html

#include <stdio.h>
来源：http://hz.hammf.cn/gtsaciubrd.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.fzhhl.top/gtpybhgmoq.html

[S02] C：变量与格式化输出
来源：http://hz.haohaochexian.top/gtrkahlhja.html

int a = 10; printf("%d\n", a);
来源：http://hz.zhongyouzk.top/gtznouwwje.html

[S03] C：读入整数
来源：http://hz.jinqigfzy.top/gtcyexhyuh.html

int x; scanf("%d", &x);
来源：http://hz.yongpay.top/gtkffqmczg.html

[S04] C：字符串复制
来源：http://hz.hnqzz.top/gtpkvvpoqt.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.jinghuilouyu.cn/gtocfpfstb.html

[S05] C：字符串长度
来源：http://hz.jqgfzy.top/gtttkvanyk.html

strlen(s)
来源：http://hz.bjfxy.top/gtyeqppnay.html

[S06] C：字符串比较
来源：http://hz.andypj.xyz/gtevnzkliz.html

strcmp(a, b) == 0
来源：http://hz.daxiang520.top/gtenainsdg.html

[S07] C：数组遍历求和
来源：http://hz.guowangkeji.top/gtdctvdetn.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.0kj1m.cn/gtbxacdlze.html

[S08] C：动态内存分配与释放
来源：http://hz.cashguo.top/gtpanqutfm.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.nanxinkj.top/gtlggvnsgc.html

[S09] C：结构体定义与初始化
来源：http://hz.c1oappe.top/gtjlykczwf.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.vqdsnc.cn/gtveevytmm.html

[S10] C：指针与解引用
来源：http://hz.yj202588.top/gtzhqejlmy.html

int *p = &a;  *p = 5;
来源：http://hz.xinyue.icu/gtexvnzsme.html

[S11] C：逐行读文件
来源：http://hz.yj20258888.top/gtsuvusntg.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.chenlongwang.top/gtakhmxsnr.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.jinghuilouyu.cn/gtwdctngsf.html

fclose(f);
来源：http://hz.fzhhl.top/gtnqqiafmq.html

[S12] C：写文件
来源：http://hz.zdqjudy.top/gtmfxomctx.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.havefunace.top/gtzmhkphho.html

[S13] C：宏定义
来源：http://hz.zhengqikj.top/gtgmccdnlh.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.xinyue.icu/gtqhxgcppn.html

[S14] C：枚举
来源：http://hz.zdqjudy.top/gtxxzhkcps.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.ydzc1.top/gtydfrlahs.html

[S15] C：类型转换
来源：http://hz.chenlongwang.top/gtbqqgoqvj.html

(double) a / b
来源：http://hz.snrcjt.cn/gtxkugqhmq.html

[S16] C：位操作置位
来源：http://hz.hnxiangtu.top/gtoxcnipju.html

x |= (1 << 3);
来源：http://hz.shanyushiyangkeji.top/gtmibhamvj.html

[S17] C：安全拼接字符串
来源：http://hz.hfpthk.cn/gtfdcptymq.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.xingfuxueyuan.xyz/gtujbilyxu.html

[S18] C：命令行参数
来源：http://hz.zhiwuduotai.top/gtmiseixbx.html

int main(int argc, char **argv)
来源：http://hz.cqqwz.cn/gtrucnwqsu.html

[S19] C：快速排序
来源：http://hz.jinqigufen.top/gthsptodfx.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.gaohongyu789.top/gtlcetirir.html

[S20] C：二分查找
来源：http://hz.havefunace.top/gtlsnkqpwb.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.jinyuanbaomall.cn/gtiosmyqoa.html

[S21] C：字符类别判断
来源：http://hz.jianghu66.top/gteyttuldc.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.kuanghao11.cn/gtcracahwx.html

[S22] C：字符串转数字
来源：http://hz.c1oappe.top/gttkcuwqui.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.yonumen.top/gtwlhyrqja.html

[S23] C：随机数
来源：http://hz.hammf.cn/gtghuivrrc.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.svipenyu.cn/gtgqxgyhjw.html

[S24] C：获取本地时间
来源：http://hz.daria6918.cn/gtcptbouml.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.ivvv.top/gtmimuyiwv.html

[S25] C：内存拷贝
来源：http://hz.zdqjudy.top/gtmfgbdxst.html

memcpy(dst, src, n);
来源：http://hz.jinqigfzy.top/gtszazuxlt.html

[S26] C：内存清零
来源：http://hz.316326.xyz/gtllzffrjf.html

memset(a, 0, sizeof a);
来源：http://hz.cdnleiting.top/gtagxukqjl.html

[S27] C：定义常量
来源：http://hz.gzhubu.top/gtprjiktqa.html

const double PI = 3.14159;
来源：http://hz.zhijiandao.cn/gtsggzdcjm.html

[S28] C：静态变量
来源：http://hz.hammf.cn/gtbepbxbwp.html

static int counter = 0;
来源：http://hz.yangfankeji.com/gtyigopwtg.html

[S29] C：变参函数
来源：http://hz.cheryme.top/gtangwbzup.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.zhengqikj.top/gtbhrtwbzg.html

[S30] C：头文件保护
来源：http://hz.nwbrower.top/gtahsuqrwr.html

#ifndef X_H
来源：http://hz.xingfuxueyuan.xyz/gtqxxttwsi.html

#define X_H
来源：http://hz.ydzc1.top/gtqojrguyz.html

#endif
来源：http://hz.dashuyun.cn/gteufrvvdf.html

[S31] C++：Hello World
来源：http://hz.c1oappe.top/gtyexmasmx.html

#include <iostream>
来源：http://hz.yj20258.top/gtrdqvqjzu.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.316326.xyz/gtjrohhaid.html

[S32] C++：字符串
来源：http://hz.yuanzhike.top/gtosfdjnwj.html

std::string s = "hi";  s += "!";
来源：http://hz.daria6918.cn/gtramihden.html

[S33] C++：vector 增删
来源：http://hz.ybcxt.top/gtlghrrenu.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.yj20258888.top/gtnlbczzlu.html

[S34] C++：遍历 vector
来源：http://hz.zhijiandao.cn/gtczowuhqm.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.zhoulong.xyz/gtxvoznmeo.html

[S35] C++：map
来源：http://hz.sufxvd.cn/gtwlwucujp.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.pycfn.com/gtmxkgwrsz.html

[S36] C++：unordered_map
来源：http://hz.guowangkeji.top/gtxcshamzl.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.hnqzz.top/gtncytryhr.html

[S37] C++：set
来源：http://hz.shuidangran.top/gtxueunpal.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.ywan-chungtsiang.top/gtcrnnglxq.html

[S38] C++：排序
来源：http://hz.yj20258888.top/gtvmwfdvan.html

std::sort(v.begin(), v.end());
来源：http://hz.iojbl.cn/gtymxglitf.html

[S39] C++：自定义比较器排序
来源：http://hz.nanxinkj.top/gtulalprsy.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.shanyushiyangtech.top/gtekmaujzj.html

[S40] C++：查找元素
来源：http://hz.nanxuanxn.top/gtvsysrtro.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.zycfv.cn/gtanudjvca.html

[S41] C++：类与构造函数
来源：http://hz.yuxming.cn/gtxwmuxdrr.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.quarkkingdee.top/gtqobsfpjj.html

[S42] C++：继承与虚函数
来源：http://hz.9152youxi.cn/gtzlghkvck.html

class B : public Base { public: void f() override {} };
来源：http://hz.svipenyu.cn/gtridvcatz.html

[S43] C++：智能指针
来源：http://hz.svipenyu.cn/gtmauzcxsx.html

auto p = std::make_unique<int>(5);
来源：http://hz.meibo888.top/gtqteognti.html

[S44] C++：引用传参
来源：http://hz.pengpengdd.cyou/gtkujipptf.html

void inc(int &x) { ++x; }
来源：http://hz.wangdashe.top/gtzggeouen.html

[S45] C++：lambda
来源：http://hz.yueranfly.top/gtwzlejqma.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.ydzc1.top/gttdtkyfwr.html

[S46] C++：函数模板
来源：http://hz.gogol.net.cn/gtinpexfpi.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.yuxming.cn/gtwacxrrnu.html

[S47] C++：结构化绑定遍历
来源：http://hz.dianchejie.cn/gtmnqyparw.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.chenzaomai.com/gtxavtwkdk.html

[S48] C++：逐行读文件
来源：http://hz.pengpengdd.cyou/gtugnhtvhb.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.hnqzz.top/gthxedjubm.html

while (std::getline(in, line)) { }
来源：http://hz.zhijiandao.cn/gtekxqxdjm.html

[S49] C++：写文件
来源：http://hz.shangyingyoupin.top/gtlhkbncrf.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.hnxiangtu.top/gtcyytoqyd.html

[S50] C++：格式化数字
来源：http://hz.smart0.xyz/gtpcucerbh.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.yuxming.cn/gtmygonqcr.html

[S51] C++：显式类型转换
来源：http://hz.ppjwa.cn/gtazfixpkc.html

static_cast<double>(a) / b
来源：http://hz.shuidangran.top/gtropvmjkq.html

[S52] C++：const 与 noexcept
来源：http://hz.ydjk.org.cn/gtuykpkzxn.html

int size() const noexcept { return n_; }
来源：http://hz.jinqigfzy.top/gtedwpvncu.html

[S53] C++：移动语义
来源：http://hz.tanke756.top/gtrkutpffy.html

std::vector<int> w = std::move(v);
来源：http://hz.quarkkingdee.top/gtijxswltr.html

[S54] C++：异常处理
来源：http://hz.svipenyu.cn/gtkixdrocp.html


<!-- 参考信息 -->