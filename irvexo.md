代发 wailian999

[Q80] 字符串截取
来源：http://hz.iojbl.cn/gtjoahzccp.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.redwolf501.top/gtyffnnker.html

[Q81] 字符串替换
来源：http://hz.jiagoushi.top/gtxzvuvyho.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.quarkkingdee.top/gtjfnxtdzk.html

[Q82] 字符长度与字节长度
来源：http://hz.jianghu66.top/gtlavdhpxy.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.aibaodan.cn/gtoowktmhs.html

[Q83] 大小写转换
来源：http://hz.haohaochexian.top/gtfufspszk.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.meibo888.top/gtkpwuchdp.html

[Q84] 去除首尾空格
来源：http://hz.shanyushiyangkeji.top/gtskkewznv.html

SELECT TRIM(name) FROM users;
来源：http://hz.wangshuangyany.cn/gtcbyvzjgb.html

[Q85] 数值取整
来源：http://hz.yj20258.top/gtlyumrexw.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.jinqigfzy.top/gtugssjvky.html

[Q86] 读取 JSON 字段
来源：http://hz.nwbrower.top/gtlmsxbdug.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.jiagoushi.top/gtezydnobe.html

[Q87] JSON 字段做条件
来源：http://hz.hywenlv.cn/gtbbtnnerk.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.feifeiyinyue.top/gtgytnxesn.html

[Q88] 行转列（条件聚合）
来源：http://hz.52xcode.cn/gtnqydlsnm.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.gaohongyu789.top/gtdutfxgve.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.bjfxy.top/gtmawlvssb.html

[Q89] 判断表是否存在
来源：http://hz.cdnleiting.top/gtczieosez.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.zhengqikj.top/gthubjicoe.html

[Q90] 生成序号列
来源：http://hz.feifeiyinyue.top/gtkviauoro.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.chenlongwang.top/gtvsjhinml.html

================================================================================
来源：http://hz.9152youxi.cn/gtvrfighwe.html

R. Bash 专题
来源：http://hz.xziqi.cn/gtzllqdipp.html

================================================================================
来源：http://hz.yuxming.cn/gtvwevgkfu.html

[R01] shebang 与严格模式
来源：http://hz.shanyushiyangtech.top/gtxivckhoo.html

#!/usr/bin/env bash
来源：http://hz.316326.xyz/gtlghagwxj.html

set -euo pipefail
来源：http://hz.yj202588.top/gtrvwyxjcy.html

[R02] 变量赋值与使用
来源：http://hz.ydzc1.top/gtahcldfmy.html

name="Tom"; echo "$name"
来源：http://hz.yuxming.cn/gtjatyehbo.html

[R03] 只读变量
来源：http://hz.yueranfly.top/gtekjkmbov.html

readonly PI=3.14
来源：http://hz.yvedp.cn/gthchefokw.html

[R04] 位置参数
来源：http://hz.vqdsnc.cn/gtrmpwkybo.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.xinyue.icu/gtgxumidjr.html

[R05] 参数默认值
来源：http://hz.jinyuanbaomall.cn/gtcxwjnxib.html

name="${1:-default}"
来源：http://hz.daxiang520.top/gtuilxzihh.html

[R06] 判断命令是否存在
来源：http://hz.meibo888.top/gtenxkvaji.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.xingfuxueyuan.xyz/gtiozwyhvh.html

[R07] if 判断文件
来源：http://hz.yvedp.cn/gtwpnfceal.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.gzhubu.top/gtjqubkbam.html

[R08] 数值比较
来源：http://hz.ydzc1.top/gthgjtqtnk.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.guannengcc.top/gtrvwuuyjs.html

[R09] 字符串比较
来源：http://hz.hfpthk.cn/gtegetdont.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.zhengqikj.top/gthnsalzeq.html

[R10] 正则匹配
来源：http://hz.ydzc1.top/gtnqbgsnyk.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.nwbrower.top/gtycmqigyy.html

[R11] case 多分支
来源：http://hz.zhaomingkeji.xyz/gtzyjwzwro.html

case "$1" in
来源：http://hz.hnxiangtu.top/gtfzechuaq.html

start) echo "启动" ;;
来源：http://hz.0kj1m.cn/gtgybfbdtc.html

stop)  echo "停止" ;;
来源：http://hz.yuanzhike.top/gtmwfqhwof.html

*)     echo "未知命令" ;;
来源：http://hz.ehwqpu.com/gthfyzeknd.html

esac
来源：http://hz.yuxming.cn/gtmidrudmi.html

[R12] for 遍历文件
来源：http://hz.iojbl.cn/gtzekapvaj.html

for f in *.txt; do echo "$f"; done
来源：http://hz.nanxuanxn.top/gtkauppgft.html

[R13] for 计数循环
来源：http://hz.mhx1999.top/gtqfdrlbrl.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.sufxvd.cn/gtyuviobbr.html

[R14] C 风格 for
来源：http://hz.vqdsnc.cn/gtucathsek.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.daria6918.cn/gtccfwwubb.html

[R15] while 逐行读文件
来源：http://hz.svipenyu.cn/gtstgikkpx.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.tian-w.cn/gtjfnadgrj.html

[R16] until 等待条件
来源：http://hz.ydzc1.top/gtbnmqxzwt.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.andypj.xyz/gtuamnlfxw.html

[R17] 数组定义与取值
来源：http://hz.pengpengdd.cyou/gtdlczoduq.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.yj20258888.top/gtiecdtcrp.html

[R18] 遍历数组
来源：http://hz.zhongyouzk.top/gtdplhvcyz.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.zdqjudy.top/gtykwkotgi.html

[R19] 数组长度
来源：http://hz.hfpthk.cn/gtblcllxkr.html

echo "${#arr[@]}"
来源：http://hz.svipenyu.cn/gtrszbdlke.html

[R20] 关联数组（字典）
来源：http://hz.pengpengdd.cyou/gtlheqzpni.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.fengsongda.top/gtgahvzrej.html

[R21] 字符串长度
来源：http://hz.snrcjt.cn/gtdhhyqiip.html

echo "${#s}"
来源：http://hz.yonumen.top/gtpargyqez.html

[R22] 截取子串
来源：http://hz.guannengcc.top/gtrfwxrqqa.html

echo "${s:0:5}"
来源：http://hz.yanxiufei.cn/gtphgqjywm.html

[R23] 字符串替换
来源：http://hz.jyoumei.cn/gtqearwjnw.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.shzxlz.cn/gtnzdsruom.html

[R24] 大小写转换
来源：http://hz.aizwys.cn/gtqercdvsf.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.yj20258888.top/gtizfnyrdh.html

[R25] 去后缀 / 去前缀
来源：http://hz.pycfn.com/gtwxtkereh.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.jiagoushi.top/gtavxzmtxd.html

[R26] 命令替换
来源：http://hz.shuidangran.top/gtqqqcswks.html

now=$(date +%F); echo "$now"
来源：http://hz.quarkkingdee.top/gtfgnmbklo.html

[R27] 算术展开
来源：http://hz.tanke756.top/gtyrbjmosx.html

echo $((1 + 2 * 3))
来源：http://hz.zhongyouzk.top/gtiefgffnl.html

[R28] 浮点运算
来源：http://hz.vqdsnc.cn/gthjkhvffh.html

echo "scale=2; 10/3" | bc
来源：http://hz.zdqjudy.top/gtxhsoenmb.html

[R29] 定义函数
来源：http://hz.gogol.net.cn/gtwmdxokud.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.sufxvd.cn/gtgqvjnetz.html

[R30] 函数返回状态码
来源：http://hz.xylfe.cn/gtipoktozr.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.tanke756.top/gtlhxuhoof.html

[R31] 局部变量
来源：http://hz.cheryme.top/gtgprjtztx.html

f() { local x=1; echo "$x"; }
来源：http://hz.mhx1999.top/gtojjfbxfi.html

[R32] 参数个数校验
来源：http://hz.jinqigfzy.top/gttxqwpybn.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.jinqigfzy.top/gtbqknixao.html

[R33] 捕获错误并提示行号
来源：http://hz.gotoacloud.top/gtxzmltpxv.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.jinqigfzy.top/gtwghnyfoi.html

[R34] 退出时清理
来源：http://hz.havefunace.top/gtuyroqwmw.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.hnxiangtu.top/gtnjwaighn.html

[R35] 后台执行并等待
来源：http://hz.daria6918.cn/gtdpwszrgz.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.hammf.cn/gtiihzvois.html

[R36] 并发执行多个任务
来源：http://hz.gzhubu.top/gtjbtkullo.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.zycfv.cn/gtrxmimpck.html

[R37] 把输出赋给变量
来源：http://hz.cashguo.top/gtvarwqxup.html

files=$(ls -1)
来源：http://hz.shanyushiyangkeji.top/gtbxhghntl.html

[R38] 管道串联
来源：http://hz.hnxiangtu.top/gtimqvastq.html

cat a.txt | grep -i error | wc -l
来源：http://hz.hfpthk.cn/gtozbxbzxi.html

[R39] 重定向标准输出与错误
来源：http://hz.nanxuanxn.top/gtluekrhhk.html

cmd > out.log 2>&1
来源：http://hz.jinghuilouyu.cn/gtymcjvkkn.html

[R40] 追加写日志
来源：http://hz.feifeiyinyue.top/gtdnkbvibk.html

echo "log" >> out.log
来源：http://hz.sweek.top/gtvqalvpgh.html

[R41] 丢弃输出
来源：http://hz.sxryk.cn/gtbjenlcqb.html

cmd >/dev/null 2>&1
来源：http://hz.yanxiufei.cn/gtlfkymupi.html

[R42] 输入重定向
来源：http://hz.0kj1m.cn/gtulhqemdm.html

wc -l < a.txt
来源：http://hz.c1oappe.top/gtragxkqlw.html

[R43] 按名字查找文件
来源：http://hz.zhongyouzk.top/gtbvlhfvwn.html

find . -name "*.log" -type f
来源：http://hz.gogol.net.cn/gtojlfygkm.html

[R44] 按修改时间查找
来源：http://hz.cashguo.top/gtjqvbtkdo.html

find . -mtime -7 -type f
来源：http://hz.pycfn.com/gteekxwsji.html

[R45] 批量删除
来源：http://hz.sweek.top/gtuvmiwzvp.html

find . -name "*.tmp" -delete
来源：http://hz.xuetiantiany.cn/gtnshqxdrr.html

[R46] 递归替换文件内容
来源：http://hz.gaohongyu789.top/gtkcipkmjz.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.ybcxt.top/gttpnebbha.html

[R47] sed 单行替换
来源：http://hz.smart0.xyz/gthjnfvvoj.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.ppjwa.cn/gtedzqesgd.html

[R48] awk 取指定列
来源：http://hz.ywan-chungtsiang.top/gtejpashhd.html

awk '{print $1, $3}' a.txt
来源：http://hz.shanyushiyangkeji.top/gtqpvydvmq.html

[R49] awk 带条件
来源：http://hz.ydzc1.top/gtueyrwxzm.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.jinqigufen.top/gtwmfpnpfi.html

[R50] awk 求和
来源：http://hz.svipenyu.cn/gtnpbauawi.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.fengsongda.top/gtfhocgzgj.html

[R51] 排序去重取前几
来源：http://hz.yj20258.top/gtwupquaai.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.0kj1m.cn/gtjizyfenp.html

[R52] 统计行数
来源：http://hz.xuetiantiany.cn/gtssqcfjml.html

wc -l a.txt
来源：http://hz.svipenyu.cn/gtthebzjiu.html

[R53] 查看文件头与实时尾
来源：http://hz.tanke756.top/gtmkoghfnc.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.xuetiantiany.cn/gtjzkptcgf.html

[R54] 比较两个文件
来源：http://hz.tanke756.top/gtbiqhdekh.html

diff a.txt b.txt
来源：http://hz.haohaochexian.top/gtiswfornr.html

[R55] 压缩与解压
来源：http://hz.shangyingyoupin.top/gtmkrprmor.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.nwbrower.top/gtvfahilry.html

[R56] 远程拷贝
来源：http://hz.pycfn.com/gtohoraqfk.html

scp file user@host:/path/
来源：http://hz.vqdsnc.cn/gtragrwwzx.html

[R57] 远程执行命令
来源：http://hz.bjfxy.top/gtithrjlcd.html

ssh user@host 'uptime'
来源：http://hz.shzxlz.cn/gtxkxzvqgi.html

[R58] 下载文件
来源：http://hz.shzxlz.cn/gtgkpztfej.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.hnxiangtu.top/gtttyvpmqt.html

[R59] 发 POST JSON
来源：http://hz.pycfn.com/gthujcdney.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.bjfxy.top/gtefwnkykv.html

[R60] 只看 HTTP 状态码
来源：http://hz.gotoacloud.top/gtlcujzuzp.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.ivvv.top/gtgahaftop.html

[R61] 磁盘占用
来源：http://hz.zycfv.cn/gtfdtrwqtz.html

df -h;  du -sh *
来源：http://hz.daria6918.cn/gtisesohmj.html

[R62] 找最占空间的文件
来源：http://hz.cheryme.top/gtobiaihhf.html

du -ah . | sort -rh | head -10
来源：http://hz.316326.xyz/gtdlwzxffh.html

[R63] 内存与进程
来源：http://hz.hnqzz.top/gttgaiwqgv.html

free -h;  ps aux | grep nginx
来源：http://hz.9152youxi.cn/gtkkepaxks.html

[R64] 结束进程
来源：http://hz.jyoumei.cn/gtmssersia.html

kill -9 $(pgrep -f app.py)
来源：http://hz.mhx1999.top/gtmsjlpzfe.html

[R65] 查看端口占用
来源：http://hz.nanxuanxn.top/gtqsgexcyw.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.redwolf501.top/gtzoohnpik.html

[R66] 定时任务
来源：http://hz.smart0.xyz/gtfxahlydw.html

crontab -e;  crontab -l
来源：http://hz.sxryk.cn/gtgsukijrt.html

[R67] 生成随机十六进制串
来源：http://hz.cheryme.top/gtglttyuhb.html

openssl rand -hex 16
来源：http://hz.ybcxt.top/gtctwyjvds.html

[R68] 计算文件校验值
来源：http://hz.9152youxi.cn/gtaalzsvek.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.xuanzx.com/gtexjghefl.html

[R69] 生成随机密码
来源：http://hz.wangshuangyany.cn/gttgegwxiv.html

head -c 16 /dev/urandom | base64
来源：http://hz.shzxlz.cn/gtncxayetk.html

[R70] 时间戳与互转
来源：http://hz.nwbrower.top/gtekfzznod.html

date +%s;  date -d @1700000000
来源：http://hz.yj20258.top/gtlkjxkeie.html

[R71] 日期格式化
来源：http://hz.yvedp.cn/gtoiwuedny.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.jqgfzy.top/gtokdgkpoq.html

[R72] 等待端口就绪
来源：http://hz.zycfv.cn/gtimidjntl.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.daria6918.cn/gtbdcizigs.html

[R73] 分割大日志
来源：http://hz.shuidangran.top/gtrsxnuubr.html

split -l 1000 big.log part_
来源：http://hz.aizwys.cn/gtpjbxpuhg.html

[R74] 批量重命名
来源：http://hz.cucudq.cn/gtkvlfonmf.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.yj20258.top/gtgcocmswt.html

[R75] 导出环境变量
来源：http://hz.cucudq.cn/gtqbycxakv.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.havefunace.top/gtztkdhxki.html

[R76] 使用临时文件
来源：http://hz.ywan-chungtsiang.top/gtzjfwrxyd.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.gaohongyu789.top/gtvowkguxl.html

[R77] 读取用户输入
来源：http://hz.redwolf501.top/gtutapbcxf.html

read -rp "请输入: " ans
来源：http://hz.sxryk.cn/gtbvrvkycx.html

[R78] 交互式菜单
来源：http://hz.yueranfly.top/gtcycsyetn.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.xingfuxueyuan.xyz/gtaqnhqugj.html

[R79] 解析命令行选项
来源：http://hz.ppjwa.cn/gtekwoylrt.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.9152youxi.cn/gtqkhfoktb.html

[R80] 查看脚本执行耗时
来源：http://hz.zdqjudy.top/gtcetganpv.html

time ./run.sh
来源：http://hz.guowangkeji.top/gtqglkxuox.html

================================================================================
来源：http://hz.jinqigufen.top/gtqrkrxvby.html

S. C / C++ 专题
来源：http://hz.yuxming.cn/gtltvvuddb.html

================================================================================
来源：http://hz.wangdashe.top/gtvxifzsaj.html

[S01] C：Hello World
来源：http://hz.dashuyun.cn/gtdhnbdhrq.html

#include <stdio.h>
来源：http://hz.guowangkeji.top/gtgtpwnhis.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.mhx1999.top/gtjbzxyxby.html

[S02] C：变量与格式化输出
来源：http://hz.aibaodan.cn/gtfuwmfwlf.html

int a = 10; printf("%d\n", a);
来源：http://hz.shanyushiyangkeji.top/gtuttrnzaq.html

[S03] C：读入整数
来源：http://hz.shangyingyoupin.top/gtggkcdapg.html

int x; scanf("%d", &x);
来源：http://hz.jinqigufen.top/gtpyicbynu.html

[S04] C：字符串复制
来源：http://hz.chenlongwang.top/gtgwkrcqtm.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.haohaochexian.top/gtxilslnub.html

[S05] C：字符串长度
来源：http://hz.gotoacloud.top/gtptdscxgk.html

strlen(s)
来源：http://hz.quarkkingdee.top/gtkcjwimri.html

[S06] C：字符串比较
来源：http://hz.zhongyouzk.top/gtmcdrepia.html

strcmp(a, b) == 0
来源：http://hz.wangdashe.top/gtnnekzkgn.html

[S07] C：数组遍历求和
来源：http://hz.yvedp.cn/gtrduheotc.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.gogol.net.cn/gthleqbpaw.html

[S08] C：动态内存分配与释放
来源：http://hz.chenjidiqi.icu/gtbpqgpdiu.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.yvedp.cn/gtarfymbxl.html

[S09] C：结构体定义与初始化
来源：http://hz.jinqigfzy.top/gtupatipsq.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.yonumen.top/gtrohycrra.html

[S10] C：指针与解引用
来源：http://hz.jlsjyb.cn/gtlseewyxq.html

int *p = &a;  *p = 5;
来源：http://hz.sxryk.cn/gtfreuqtna.html

[S11] C：逐行读文件
来源：http://hz.gotoacloud.top/gtrvnmbvrv.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.xingfuxueyuan.xyz/gtbzvpgvma.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.shuidangran.top/gtpyxwobof.html

fclose(f);
来源：http://hz.cdnleiting.top/gtxsiiizzz.html

[S12] C：写文件
来源：http://hz.haohaochexian.top/gtqgkddsla.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.tanke756.top/gtbtfgdktb.html

[S13] C：宏定义
来源：http://hz.sufxvd.cn/gtwbwhjvqh.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.ivvv.top/gtkabaubyo.html

[S14] C：枚举
来源：http://hz.ybcxt.top/gttlsfysyn.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.tanke756.top/gtpojuocxg.html

[S15] C：类型转换
来源：http://hz.yvedp.cn/gtzywoiwcb.html

(double) a / b
来源：http://hz.xziqi.cn/gtotlfbxyt.html

[S16] C：位操作置位
来源：http://hz.chenzaomai.com/gtesrxycoq.html

x |= (1 << 3);
来源：http://hz.aibaodan.cn/gtcwrwgrjm.html

[S17] C：安全拼接字符串
来源：http://hz.smart0.xyz/gtisdtlkcs.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.zhijiandao.cn/gtvdzmfucr.html

[S18] C：命令行参数
来源：http://hz.xuetiantiany.cn/gtoxxxjdje.html

int main(int argc, char **argv)
来源：http://hz.zycfv.cn/gtrkfbghwn.html

[S19] C：快速排序
来源：http://hz.snrcjt.cn/gtmhgjgrtb.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.nanxinkj.top/gteapmvwfc.html

[S20] C：二分查找
来源：http://hz.shangyingyoupin.top/gtgdsiximq.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.zhoulong.xyz/gtzvpyljue.html

[S21] C：字符类别判断
来源：http://hz.zhijiandao.cn/gtvmifzwea.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.c1oappe.top/gtzohrnhdm.html

[S22] C：字符串转数字
来源：http://hz.zhengqikj.top/gtmqamseuj.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.feifeiyinyue.top/gtcknyhcea.html

[S23] C：随机数
来源：http://hz.quarkkingdee.top/gtwsemuuwc.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.pengpengdd.cyou/gtsrujeegg.html

[S24] C：获取本地时间
来源：http://hz.jyoumei.cn/gtlmkfblyp.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.daxiang520.top/gticrisqhj.html

[S25] C：内存拷贝
来源：http://hz.havefunace.top/gtvhkqinzq.html

memcpy(dst, src, n);
来源：http://hz.c1oappe.top/gtjiowzrze.html

[S26] C：内存清零
来源：http://hz.zhiwuduotai.top/gtxctjypmg.html

memset(a, 0, sizeof a);
来源：http://hz.tianlin.xyz/gtujfflggp.html

[S27] C：定义常量
来源：http://hz.hammf.cn/gtamemctls.html

const double PI = 3.14159;
来源：http://hz.zhongyouzk.top/gtqgbcwimx.html

[S28] C：静态变量
来源：http://hz.ydjk.org.cn/gtmkhpfhth.html

static int counter = 0;
来源：http://hz.shanyushiyangkeji.top/gtmdrfiuyg.html

[S29] C：变参函数
来源：http://hz.zhijiandao.cn/gthctoiwku.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.cqqwz.cn/gtvgotgjst.html

[S30] C：头文件保护
来源：http://hz.chenzaomai.com/gtpjrnihvv.html

#ifndef X_H
来源：http://hz.snrcjt.cn/gthempxron.html

#define X_H
来源：http://hz.yonumen.top/gtyuiexwgj.html

#endif
来源：http://hz.hysaishi.cn/gtbvxcpstx.html

[S31] C++：Hello World
来源：http://hz.c1oappe.top/gtuczwvolt.html

#include <iostream>
来源：http://hz.xingfuxueyuan.xyz/gtnqevyfpp.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.c1oappe.top/gtmgwzlxst.html

[S32] C++：字符串
来源：http://hz.hfpthk.cn/gtezfyrlls.html

std::string s = "hi";  s += "!";
来源：http://hz.andypj.xyz/gtcixcuhgp.html

[S33] C++：vector 增删
来源：http://hz.xuanzx.com/gtmreneuou.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.xinyue.icu/gtdwncuhrw.html

[S34] C++：遍历 vector
来源：http://hz.gogol.net.cn/gtuhqphkys.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.aizwys.cn/gtcgqwkyyt.html

[S35] C++：map
来源：http://hz.jqgfzy.top/gtovqseqfv.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.xingfuxueyuan.xyz/gtcvzpfggy.html

[S36] C++：unordered_map
来源：http://hz.c1oappe.top/gtzmcgpzqt.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.tianlin.xyz/gtvsicfzlo.html

[S37] C++：set
来源：http://hz.gzhubu.top/gtqqqtnvlk.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.chenjidiqi.icu/gtmozwmfjd.html

[S38] C++：排序
来源：http://hz.yj20258.top/gtxqcobgjx.html

std::sort(v.begin(), v.end());
来源：http://hz.fzhhl.top/gtgcnhogft.html

[S39] C++：自定义比较器排序
来源：http://hz.shuidangran.top/gtvcymcwyo.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.yueranfly.top/gtdqatzebs.html

[S40] C++：查找元素
来源：http://hz.birdmap.top/gtkawavwml.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.iojbl.cn/gtvfbfleja.html

[S41] C++：类与构造函数
来源：http://hz.shuidangran.top/gtaztkqkzf.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.daxiang520.top/gtkhjziytv.html

[S42] C++：继承与虚函数
来源：http://hz.chenjidiqi.icu/gtdcwdiydk.html

class B : public Base { public: void f() override {} };
来源：http://hz.yangfankeji.com/gtrgnjfyzb.html

[S43] C++：智能指针
来源：http://hz.yongpay.top/gtnjkotrvi.html

auto p = std::make_unique<int>(5);
来源：http://hz.pycfn.com/gtpsysdjae.html

[S44] C++：引用传参
来源：http://hz.daria6918.cn/gthganylad.html

void inc(int &x) { ++x; }
来源：http://hz.yj20258888.top/gtfynhiosd.html

[S45] C++：lambda
来源：http://hz.wangdashe.top/gtgvxhceks.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.pengpengdd.cyou/gtchxrwqam.html

[S46] C++：函数模板
来源：http://hz.sxryk.cn/gtbdreypuw.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.nanxuanxn.top/gtekojqebf.html

[S47] C++：结构化绑定遍历
来源：http://hz.andypj.xyz/gtkxwzpfoe.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.shanyushiyangtech.top/gtrscgjfmp.html

[S48] C++：逐行读文件
来源：http://hz.xuanzx.com/gthnytuozz.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.snrcjt.cn/gtimzoofje.html

while (std::getline(in, line)) { }
来源：http://hz.jiagoushi.top/gtkwsjfrxb.html

[S49] C++：写文件
来源：http://hz.wangdashe.top/gtvrliajdq.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.guowangkeji.top/gtzxujlzwx.html

[S50] C++：格式化数字
来源：http://hz.tian-w.cn/gtzhxpbntn.html


<!-- 参考信息 -->