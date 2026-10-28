代发 wailian999

[Q82] 字符长度与字节长度
来源：http://hz.ydjk.org.cn/gtcdwealot.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.yj202588.top/gtsdvynrec.html

[Q83] 大小写转换
来源：http://hz.yvedp.cn/gthqwtdtrf.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.guowangkeji.top/gtkurwflhd.html

[Q84] 去除首尾空格
来源：http://hz.sufxvd.cn/gtzwqzofcz.html

SELECT TRIM(name) FROM users;
来源：http://hz.zdqjudy.top/gttblcpchj.html

[Q85] 数值取整
来源：http://hz.yanxiufei.cn/gtrflzpucu.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.zycfv.cn/gtaxmljnqi.html

[Q86] 读取 JSON 字段
来源：http://hz.zycfv.cn/gtevkgaxyb.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.meibo888.top/gttkruvbyf.html

[Q87] JSON 字段做条件
来源：http://hz.xinyue.icu/gtsdflrnrg.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.ydzc1.top/gtzaknjszu.html

[Q88] 行转列（条件聚合）
来源：http://hz.xziqi.cn/gtupampniy.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.shanyushiyangkeji.top/gtgrxbdzla.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.gzhubu.top/gtdhedrrsc.html

[Q89] 判断表是否存在
来源：http://hz.fengsongda.top/gtdayutsbh.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.jlsjyb.cn/gtrwakdxuf.html

[Q90] 生成序号列
来源：http://hz.chenzaomai.com/gtqyyditre.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.ehwqpu.com/gtqmnirgcz.html

================================================================================
来源：http://hz.hnqzz.top/gtxtcbyhdp.html

R. Bash 专题
来源：http://hz.ppjwa.cn/gtelzonqkd.html

================================================================================
来源：http://hz.zhongyouzk.top/gtqwazkrlt.html

[R01] shebang 与严格模式
来源：http://hz.haohaochexian.top/gtvebyiakz.html

#!/usr/bin/env bash
来源：http://hz.c1oappe.top/gtbvmemgjp.html

set -euo pipefail
来源：http://hz.zhixingplan.top/gtmrxkckjb.html

[R02] 变量赋值与使用
来源：http://hz.shanyushiyangtech.top/gtntdqjfac.html

name="Tom"; echo "$name"
来源：http://hz.wangshuangyany.cn/gtalgexzsa.html

[R03] 只读变量
来源：http://hz.nwbrower.top/gtktuadfbo.html

readonly PI=3.14
来源：http://hz.ehwqpu.com/gteskopbch.html

[R04] 位置参数
来源：http://hz.pycfn.com/gtsuimmpxk.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.jinghuilouyu.cn/gtrptmxzat.html

[R05] 参数默认值
来源：http://hz.wangdashe.top/gtmzeiixvp.html

name="${1:-default}"
来源：http://hz.aizwys.cn/gtcvmyxvgu.html

[R06] 判断命令是否存在
来源：http://hz.yanxiufei.cn/gtulpndzfx.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.fengsongda.top/gtybdbvvrl.html

[R07] if 判断文件
来源：http://hz.zhiwuduotai.top/gtfilehoue.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.tianlin.xyz/gtrlqzbodd.html

[R08] 数值比较
来源：http://hz.jlsjyb.cn/gtzgdnhwlg.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.xingfuxueyuan.xyz/gtxdiqcypf.html

[R09] 字符串比较
来源：http://hz.cashguo.top/gtwtjmbrod.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.aibaodan.cn/gtzqiykbmd.html

[R10] 正则匹配
来源：http://hz.pengpengdd.cyou/gticqfzazn.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.hysaishi.cn/gtkscxlnet.html

[R11] case 多分支
来源：http://hz.0kj1m.cn/gtwxqbyjit.html

case "$1" in
来源：http://hz.dianchejie.cn/gtzpcpczfh.html

start) echo "启动" ;;
来源：http://hz.c1oappe.top/gtgtustwui.html

stop)  echo "停止" ;;
来源：http://hz.yj20258.top/gtefdveuig.html

*)     echo "未知命令" ;;
来源：http://hz.jinghuilouyu.cn/gtlftjcczq.html

esac
来源：http://hz.meibo888.top/gtdtisnaao.html

[R12] for 遍历文件
来源：http://hz.hammf.cn/gtjvluweja.html

for f in *.txt; do echo "$f"; done
来源：http://hz.yuxming.cn/gtnmzgyica.html

[R13] for 计数循环
来源：http://hz.yongpay.top/gtgcjnoyza.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.c1oappe.top/gtwkdoscot.html

[R14] C 风格 for
来源：http://hz.jiagoushi.top/gtvdxuzgkf.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.jiagoushi.top/gtlqgdfsjv.html

[R15] while 逐行读文件
来源：http://hz.zhaomingkeji.xyz/gtmobqdckq.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.yueranfly.top/gtkuvewnws.html

[R16] until 等待条件
来源：http://hz.shanyushiyangtech.top/gtusiokuyv.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.nanxinkj.top/gtodavgnax.html

[R17] 数组定义与取值
来源：http://hz.yj20258.top/gtphsqimpr.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.9152youxi.cn/gtspyjkffc.html

[R18] 遍历数组
来源：http://hz.dashuyun.cn/gthiisnask.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.ybcxt.top/gtmvnxored.html

[R19] 数组长度
来源：http://hz.dianchejie.cn/gtyhbnbhtf.html

echo "${#arr[@]}"
来源：http://hz.zdqjudy.top/gtfpbppaeo.html

[R20] 关联数组（字典）
来源：http://hz.daxiang520.top/gtqtqqidal.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.yanxiufei.cn/gtvbjrdodx.html

[R21] 字符串长度
来源：http://hz.yangfankeji.com/gtpymbsguw.html

echo "${#s}"
来源：http://hz.birdmap.top/gtbrazieen.html

[R22] 截取子串
来源：http://hz.xuanzx.com/gtghpvqstb.html

echo "${s:0:5}"
来源：http://hz.smart0.xyz/gtzmudxakr.html

[R23] 字符串替换
来源：http://hz.chenzaomai.com/gtcymighwj.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.kuanghao11.cn/gtsutichva.html

[R24] 大小写转换
来源：http://hz.shzxlz.cn/gtawtkklmx.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.cqqwz.cn/gtemwujebj.html

[R25] 去后缀 / 去前缀
来源：http://hz.vqdsnc.cn/gtmyxzmxfp.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.nwbrower.top/gtsmvkkfpt.html

[R26] 命令替换
来源：http://hz.ydjk.org.cn/gtvarsbuau.html

now=$(date +%F); echo "$now"
来源：http://hz.pycfn.com/gtzuursjgt.html

[R27] 算术展开
来源：http://hz.0kj1m.cn/gtyshogypm.html

echo $((1 + 2 * 3))
来源：http://hz.ybcxt.top/gtegkknxdq.html

[R28] 浮点运算
来源：http://hz.havefunace.top/gtavwyqmdf.html

echo "scale=2; 10/3" | bc
来源：http://hz.gotoacloud.top/gthubnrdhb.html

[R29] 定义函数
来源：http://hz.daria6918.cn/gtwhlrnvly.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.sxryk.cn/gtdvvaczyx.html

[R30] 函数返回状态码
来源：http://hz.shangyingyoupin.top/gtmopedweh.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.pengpengdd.cyou/gtbxozzufk.html

[R31] 局部变量
来源：http://hz.aibaodan.cn/gtmvctbhps.html

f() { local x=1; echo "$x"; }
来源：http://hz.ivvv.top/gtanwgkryd.html

[R32] 参数个数校验
来源：http://hz.shuidangran.top/gtauqzzysl.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.mhx1999.top/gthljzvghs.html

[R33] 捕获错误并提示行号
来源：http://hz.shzxlz.cn/gtbdlxmaop.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.daria6918.cn/gtvqhrclzr.html

[R34] 退出时清理
来源：http://hz.sysykeji.top/gtikgkxajc.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.xylfe.cn/gtjumjozhi.html

[R35] 后台执行并等待
来源：http://hz.tanke756.top/gtrskuecxe.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.tian-w.cn/gtdwxfzhgz.html

[R36] 并发执行多个任务
来源：http://hz.havefunace.top/gtgimnrgwc.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.yongpay.top/gtgdgtogsp.html

[R37] 把输出赋给变量
来源：http://hz.jlsjyb.cn/gtarqxoxwu.html

files=$(ls -1)
来源：http://hz.dashuyun.cn/gtskjzxsfh.html

[R38] 管道串联
来源：http://hz.hywenlv.cn/gtvarvnyht.html

cat a.txt | grep -i error | wc -l
来源：http://hz.xuetiantiany.cn/gtgisxnpsq.html

[R39] 重定向标准输出与错误
来源：http://hz.bjfxy.top/gtwekxneur.html

cmd > out.log 2>&1
来源：http://hz.9152youxi.cn/gtxjzjcbna.html

[R40] 追加写日志
来源：http://hz.gotoacloud.top/gtjfyubejb.html

echo "log" >> out.log
来源：http://hz.yonumen.top/gtzlcclfld.html

[R41] 丢弃输出
来源：http://hz.chenzaomai.com/gtukhktilc.html

cmd >/dev/null 2>&1
来源：http://hz.sxryk.cn/gtilzayakw.html

[R42] 输入重定向
来源：http://hz.9152youxi.cn/gtoajaumnw.html

wc -l < a.txt
来源：http://hz.nanxuanxn.top/gtkgbjiqlm.html

[R43] 按名字查找文件
来源：http://hz.zhiwuduotai.top/gtlasrikoq.html

find . -name "*.log" -type f
来源：http://hz.zhijiandao.cn/gtdpdxyecr.html

[R44] 按修改时间查找
来源：http://hz.fzhhl.top/gtmpnxotfx.html

find . -mtime -7 -type f
来源：http://hz.316326.xyz/gthoxraxrl.html

[R45] 批量删除
来源：http://hz.feifeiyinyue.top/gtaplewkpu.html

find . -name "*.tmp" -delete
来源：http://hz.jinghuilouyu.cn/gtizkjzmnh.html

[R46] 递归替换文件内容
来源：http://hz.xingfuxueyuan.xyz/gtohzunknu.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.havefunace.top/gtrmypqixs.html

[R47] sed 单行替换
来源：http://hz.wangshuangyany.cn/gtwhqroysh.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.yj20258888.top/gtazestocn.html

[R48] awk 取指定列
来源：http://hz.yangfankeji.com/gtmawdtwxg.html

awk '{print $1, $3}' a.txt
来源：http://hz.52xcode.cn/gtedwaabzl.html

[R49] awk 带条件
来源：http://hz.daxiang520.top/gtdjniafkg.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.ppjwa.cn/gtjycicbdm.html

[R50] awk 求和
来源：http://hz.zhixingplan.top/gtwwarlfex.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.jianghu66.top/gtpkwaohqa.html

[R51] 排序去重取前几
来源：http://hz.nwbrower.top/gtdehpinrl.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.hnxiangtu.top/gtlzmsslph.html

[R52] 统计行数
来源：http://hz.jyoumei.cn/gtaoebawmd.html

wc -l a.txt
来源：http://hz.hysaishi.cn/gtmxltdjsn.html

[R53] 查看文件头与实时尾
来源：http://hz.jinyuanbaomall.cn/gtcqmjghtc.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.yuanzhike.top/gtqehogahp.html

[R54] 比较两个文件
来源：http://hz.hnqzz.top/gtnwpgqveu.html

diff a.txt b.txt
来源：http://hz.shzxlz.cn/gtxdqmndsr.html

[R55] 压缩与解压
来源：http://hz.jinghuilouyu.cn/gtuvldfdzd.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.jinqigfzy.top/gtyiclnftj.html

[R56] 远程拷贝
来源：http://hz.daria6918.cn/gtkxjmgcnw.html

scp file user@host:/path/
来源：http://hz.wangdashe.top/gtscrswcit.html

[R57] 远程执行命令
来源：http://hz.shanyushiyangkeji.top/gthogqzkha.html

ssh user@host 'uptime'
来源：http://hz.guannengcc.top/gtxrsijdfv.html

[R58] 下载文件
来源：http://hz.cheryme.top/gtugdizzuk.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.shangyingyoupin.top/gtnnouhybd.html

[R59] 发 POST JSON
来源：http://hz.zhiwuduotai.top/gtwlzszkaz.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.yj20258888.top/gtqjmmvmot.html

[R60] 只看 HTTP 状态码
来源：http://hz.hfpthk.cn/gtmfofgjeh.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.ppjwa.cn/gtsmvrpxle.html

[R61] 磁盘占用
来源：http://hz.tianlin.xyz/gthrdivfil.html

df -h;  du -sh *
来源：http://hz.wangdashe.top/gtrvqduajx.html

[R62] 找最占空间的文件
来源：http://hz.jinqigufen.top/gtsmyobtio.html

du -ah . | sort -rh | head -10
来源：http://hz.havefunace.top/gtydbjstlm.html

[R63] 内存与进程
来源：http://hz.zhijiandao.cn/gthffpphad.html

free -h;  ps aux | grep nginx
来源：http://hz.hysaishi.cn/gtgnmikhnm.html

[R64] 结束进程
来源：http://hz.gzhubu.top/gtwcmifulp.html

kill -9 $(pgrep -f app.py)
来源：http://hz.guowangkeji.top/gtysgwdueb.html

[R65] 查看端口占用
来源：http://hz.nwbrower.top/gtcdjzmzjd.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.gzhubu.top/gtnwwzrobe.html

[R66] 定时任务
来源：http://hz.0kj1m.cn/gtiwzbylbl.html

crontab -e;  crontab -l
来源：http://hz.cucudq.cn/gtkyardlkj.html

[R67] 生成随机十六进制串
来源：http://hz.jqgufenzy.top/gtsmevhrfj.html

openssl rand -hex 16
来源：http://hz.tian-w.cn/gtzpkigmld.html

[R68] 计算文件校验值
来源：http://hz.zhengqikj.top/gtazlqyswi.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.xuanzx.com/gtnuhxxena.html

[R69] 生成随机密码
来源：http://hz.yangfankeji.com/gtyogbmrgo.html

head -c 16 /dev/urandom | base64
来源：http://hz.nanxuanxn.top/gtsavbfbcg.html

[R70] 时间戳与互转
来源：http://hz.zhoulong.xyz/gtjhkuagoz.html

date +%s;  date -d @1700000000
来源：http://hz.shzxlz.cn/gtnzcoozza.html

[R71] 日期格式化
来源：http://hz.52xcode.cn/gtwrnrknmn.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.havefunace.top/gthrtlrhwh.html

[R72] 等待端口就绪
来源：http://hz.jlsjyb.cn/gtburovlto.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.zycfv.cn/gthwuvrsqv.html

[R73] 分割大日志
来源：http://hz.sweek.top/gthyltwetc.html

split -l 1000 big.log part_
来源：http://hz.zhongyouzk.top/gtvwvmetkx.html

[R74] 批量重命名
来源：http://hz.hnqzz.top/gtfpsdhifv.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.guannengcc.top/gtwwwyvbgm.html

[R75] 导出环境变量
来源：http://hz.ivvv.top/gtphiyzgqi.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.xinyue.icu/gtckrfhpck.html

[R76] 使用临时文件
来源：http://hz.jinghuilouyu.cn/gthkcslppa.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.shanyushiyangtech.top/gtxmwvydtd.html

[R77] 读取用户输入
来源：http://hz.zhixingplan.top/gtbmkdqizn.html

read -rp "请输入: " ans
来源：http://hz.yangfankeji.com/gtgzpmvdkw.html

[R78] 交互式菜单
来源：http://hz.wangshuangyany.cn/gtovwnvomd.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.9152youxi.cn/gtrtkgtsoh.html

[R79] 解析命令行选项
来源：http://hz.zhongyouzk.top/gtpascwdoj.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.chenjidiqi.icu/gtbmzxpacd.html

[R80] 查看脚本执行耗时
来源：http://hz.52xcode.cn/gtrkwzdegj.html

time ./run.sh
来源：http://hz.yuanzhike.top/gtoolgfsjv.html

================================================================================
来源：http://hz.yangfankeji.com/gthfkkwanb.html

S. C / C++ 专题
来源：http://hz.jinghuilouyu.cn/gtftweyhbg.html

================================================================================
来源：http://hz.ivvv.top/gtusubyuds.html

[S01] C：Hello World
来源：http://hz.hnqzz.top/gtpanxrrjl.html

#include <stdio.h>
来源：http://hz.xylfe.cn/gtpqrmskvl.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.gzhubu.top/gtbiukfwtz.html

[S02] C：变量与格式化输出
来源：http://hz.jqgfzy.top/gtjofsezna.html

int a = 10; printf("%d\n", a);
来源：http://hz.cheryme.top/gtvpevivtd.html

[S03] C：读入整数
来源：http://hz.cdnleiting.top/gtsoachgfh.html

int x; scanf("%d", &x);
来源：http://hz.iojbl.cn/gtxxepsdph.html

[S04] C：字符串复制
来源：http://hz.gogol.net.cn/gtwnrlubsf.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.zhongyouzk.top/gtssdacikb.html

[S05] C：字符串长度
来源：http://hz.xuetiantiany.cn/gtajwwlnii.html

strlen(s)
来源：http://hz.hongshengwenyu.top/gtfjalfnih.html

[S06] C：字符串比较
来源：http://hz.gotoacloud.top/gtynxsvfjd.html

strcmp(a, b) == 0
来源：http://hz.hnqzz.top/gtpdvnxwjv.html

[S07] C：数组遍历求和
来源：http://hz.yonumen.top/gtkthrwvia.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.fzhhl.top/gtejfjqhfk.html

[S08] C：动态内存分配与释放
来源：http://hz.yj202588.top/gtrbtxvwzy.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.tianlin.xyz/gtwddifrna.html

[S09] C：结构体定义与初始化
来源：http://hz.zdqjudy.top/gtnjywsgwk.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.zhongyouzk.top/gtojxxyego.html

[S10] C：指针与解引用
来源：http://hz.yueranfly.top/gtowbjyluh.html

int *p = &a;  *p = 5;
来源：http://hz.zhijiandao.cn/gtbewwjhfb.html

[S11] C：逐行读文件
来源：http://hz.xylfe.cn/gtoequbwfq.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.jqgufenzy.top/gtofqgedkd.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.daxiang520.top/gthmffucqq.html

fclose(f);
来源：http://hz.yonumen.top/gtnreteahp.html

[S12] C：写文件
来源：http://hz.hammf.cn/gttbgzzmrn.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.ivvv.top/gttlsyorrr.html

[S13] C：宏定义
来源：http://hz.snrcjt.cn/gtozczutux.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.tianlin.xyz/gtgqquxcgh.html

[S14] C：枚举
来源：http://hz.xingfuxueyuan.xyz/gtgpttudrl.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.fengsongda.top/gtokfwfkjg.html

[S15] C：类型转换
来源：http://hz.yj202588.top/gtebswqanb.html

(double) a / b
来源：http://hz.kuanghao11.cn/gtxiqnrler.html

[S16] C：位操作置位
来源：http://hz.jlsjyb.cn/gtkdoegjzh.html

x |= (1 << 3);
来源：http://hz.52xcode.cn/gtsyljeoqn.html

[S17] C：安全拼接字符串
来源：http://hz.cqqwz.cn/gtcyroircv.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.zycfv.cn/gtbbackfig.html

[S18] C：命令行参数
来源：http://hz.jyoumei.cn/gtkcrtxueh.html

int main(int argc, char **argv)
来源：http://hz.ppjwa.cn/gtenmdtfpk.html

[S19] C：快速排序
来源：http://hz.316326.xyz/gtlyjpxieg.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.hnxiangtu.top/gtbjsomphz.html

[S20] C：二分查找
来源：http://hz.hysaishi.cn/gtthkirpem.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.yonumen.top/gtgklgpmxc.html

[S21] C：字符类别判断
来源：http://hz.xingfuxueyuan.xyz/gtglfzjvfq.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.bjfxy.top/gtxhvpsild.html

[S22] C：字符串转数字
来源：http://hz.mhx1999.top/gtjoxzheuz.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.dianchejie.cn/gtyglknhgv.html

[S23] C：随机数
来源：http://hz.sweek.top/gtjdrbatac.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.wangdashe.top/gtqagecyus.html

[S24] C：获取本地时间
来源：http://hz.daria6918.cn/gtbsmzzsxx.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.fzhhl.top/gtlvlnkadn.html

[S25] C：内存拷贝
来源：http://hz.chenjidiqi.icu/gtyhpxbeiz.html

memcpy(dst, src, n);
来源：http://hz.shangyingyoupin.top/gtxhhbpsah.html

[S26] C：内存清零
来源：http://hz.iojbl.cn/gtvjysknoh.html

memset(a, 0, sizeof a);
来源：http://hz.havefunace.top/gtcagpkpzj.html

[S27] C：定义常量
来源：http://hz.gzhubu.top/gtdjnbihoe.html

const double PI = 3.14159;
来源：http://hz.shzxlz.cn/gtqrzzewtk.html

[S28] C：静态变量
来源：http://hz.yj202588.top/gtztzixqaa.html

static int counter = 0;
来源：http://hz.havefunace.top/gtmosprnmf.html

[S29] C：变参函数
来源：http://hz.mhx1999.top/gtstoegiqf.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.xuanzx.com/gtrqzjcuqr.html

[S30] C：头文件保护
来源：http://hz.yuxming.cn/gtqztuxdjb.html

#ifndef X_H
来源：http://hz.yonumen.top/gtyqcaonug.html

#define X_H
来源：http://hz.vqdsnc.cn/gtypkzclbb.html

#endif
来源：http://hz.chenlongwang.top/gtmegwcwno.html

[S31] C++：Hello World
来源：http://hz.dashuyun.cn/gtbvnqijzv.html

#include <iostream>
来源：http://hz.xylfe.cn/gtiocwjows.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.hammf.cn/gtnsndjsgn.html

[S32] C++：字符串
来源：http://hz.jianghu66.top/gtbjyptomh.html

std::string s = "hi";  s += "!";
来源：http://hz.hammf.cn/gtopcvvgye.html

[S33] C++：vector 增删
来源：http://hz.yj20258.top/gtxlikyfeg.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.chenlongwang.top/gtcwjxgpye.html

[S34] C++：遍历 vector
来源：http://hz.hysaishi.cn/gtujzmmoqk.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.shanyushiyangtech.top/gtjrlsurxw.html

[S35] C++：map
来源：http://hz.daxiang520.top/gtrgoygrnl.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.cdnleiting.top/gthlxddhcv.html

[S36] C++：unordered_map
来源：http://hz.shangyingyoupin.top/gtyqntrjaf.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.sweek.top/gtdogvfhrm.html

[S37] C++：set
来源：http://hz.cdnleiting.top/gtcgtjvrjw.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.kuanghao11.cn/gtchuzlbag.html

[S38] C++：排序
来源：http://hz.ppjwa.cn/gtkgjhzokh.html

std::sort(v.begin(), v.end());
来源：http://hz.nanxuanxn.top/gtzxugkywe.html

[S39] C++：自定义比较器排序
来源：http://hz.tanke756.top/gtfuyhngpb.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.wangdashe.top/gtxftshxxc.html

[S40] C++：查找元素
来源：http://hz.cdnleiting.top/gthatjcfyu.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.jyoumei.cn/gtofzfejpp.html

[S41] C++：类与构造函数
来源：http://hz.andypj.xyz/gtnsxiqfzl.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.nwbrower.top/gtawqcrtod.html

[S42] C++：继承与虚函数
来源：http://hz.yangfankeji.com/gtimkbjlpg.html

class B : public Base { public: void f() override {} };
来源：http://hz.gaohongyu789.top/gtyclrklus.html

[S43] C++：智能指针
来源：http://hz.zhongyouzk.top/gtrszycatd.html

auto p = std::make_unique<int>(5);
来源：http://hz.fengsongda.top/gtriniiodf.html

[S44] C++：引用传参
来源：http://hz.hongshengwenyu.top/gtwkukperv.html

void inc(int &x) { ++x; }
来源：http://hz.bjfxy.top/gtpqwzsyfh.html

[S45] C++：lambda
来源：http://hz.ivvv.top/gtiusudyxg.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.daria6918.cn/gtkoqbeica.html

[S46] C++：函数模板
来源：http://hz.cashguo.top/gtgcgfwblm.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.zdqjudy.top/gttjinbzkk.html

[S47] C++：结构化绑定遍历
来源：http://hz.jinqigufen.top/gtzgjexzxp.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.yonumen.top/gtaheybxfc.html

[S48] C++：逐行读文件
来源：http://hz.vqdsnc.cn/gttqxbowew.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.hongshengwenyu.top/gtyzqjtqib.html

while (std::getline(in, line)) { }
来源：http://hz.ivvv.top/gtedvjfbuu.html

[S49] C++：写文件
来源：http://hz.aizwys.cn/gtymaciard.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.bjfxy.top/gtrtngxfqj.html

[S50] C++：格式化数字
来源：http://hz.yueranfly.top/gtrojjnofl.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.sufxvd.cn/gtfldzotwk.html

[S51] C++：显式类型转换
来源：http://hz.yj20258.top/gttqdddneu.html

static_cast<double>(a) / b
来源：http://hz.hysaishi.cn/gtxtbcbvxd.html

[S52] C++：const 与 noexcept
来源：http://hz.gogol.net.cn/gtzdgsimbx.html


<!-- 参考信息 -->