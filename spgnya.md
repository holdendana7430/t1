代发 wailian999

[Q78] 当前时间
来源：http://hz.shangyingyoupin.top/gtpwxtkwlq.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.hysaishi.cn/gthdwosvse.html

[Q79] 字符串拼接
来源：http://hz.jqgfzy.top/gtlcoiaptw.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.shanyushiyangtech.top/gtejqfxoqz.html

[Q80] 字符串截取
来源：http://hz.zhiwuduotai.top/gtmdttvnsq.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.yueranfly.top/gtvsqwnrui.html

[Q81] 字符串替换
来源：http://hz.jqgufenzy.top/gtwsohtlfn.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.jqgufenzy.top/gtxwuwaurc.html

[Q82] 字符长度与字节长度
来源：http://hz.birdmap.top/gtwuwjvlcl.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.fzhhl.top/gtnzwheokv.html

[Q83] 大小写转换
来源：http://hz.vqdsnc.cn/gtdrdmyfox.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.wangshuangyany.cn/gtccyjwmtu.html

[Q84] 去除首尾空格
来源：http://hz.tanke756.top/gtdirvuavk.html

SELECT TRIM(name) FROM users;
来源：http://hz.meibo888.top/gtlxanlbga.html

[Q85] 数值取整
来源：http://hz.sufxvd.cn/gtyjqxqisj.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.guannengcc.top/gthxbynruk.html

[Q86] 读取 JSON 字段
来源：http://hz.wangshuangyany.cn/gtswdtdbml.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.chenzaomai.com/gtqjfscxyk.html

[Q87] JSON 字段做条件
来源：http://hz.jyoumei.cn/gtuvylcsno.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.guannengcc.top/gtkkiilyyb.html

[Q88] 行转列（条件聚合）
来源：http://hz.xylfe.cn/gtxuciqcnn.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.gaohongyu789.top/gtxmxvbunr.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.yj20258.top/gthmqqovbn.html

[Q89] 判断表是否存在
来源：http://hz.dianchejie.cn/gtnywbmexx.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.chenjidiqi.icu/gtkmsgykns.html

[Q90] 生成序号列
来源：http://hz.chenjidiqi.icu/gtbqyptxft.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.sufxvd.cn/gtudefrpkw.html

================================================================================
来源：http://hz.kuanghao11.cn/gtwkenjxpn.html

R. Bash 专题
来源：http://hz.yangfankeji.com/gteptcckul.html

================================================================================
来源：http://hz.snrcjt.cn/gtisoyaqlf.html

[R01] shebang 与严格模式
来源：http://hz.zhaomingkeji.xyz/gtuwaqjwsp.html

#!/usr/bin/env bash
来源：http://hz.nwbrower.top/gtkeuhwtqv.html

set -euo pipefail
来源：http://hz.dashuyun.cn/gtbkolswzs.html

[R02] 变量赋值与使用
来源：http://hz.quarkkingdee.top/gtgnemndun.html

name="Tom"; echo "$name"
来源：http://hz.fzhhl.top/gtotvwnraj.html

[R03] 只读变量
来源：http://hz.fzhhl.top/gtixtprwoj.html

readonly PI=3.14
来源：http://hz.havefunace.top/gtvueneewl.html

[R04] 位置参数
来源：http://hz.snrcjt.cn/gtourfoxzr.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.yj20258.top/gtfkexpent.html

[R05] 参数默认值
来源：http://hz.gogol.net.cn/gtngylsylw.html

name="${1:-default}"
来源：http://hz.ywan-chungtsiang.top/gtwvmdbmen.html

[R06] 判断命令是否存在
来源：http://hz.havefunace.top/gtedzytipk.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.c1oappe.top/gtqczfivki.html

[R07] if 判断文件
来源：http://hz.quarkkingdee.top/gtqihfhhdv.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.fzhhl.top/gtoogtisvj.html

[R08] 数值比较
来源：http://hz.ydjk.org.cn/gtejjxjfkk.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.shzxlz.cn/gtmsifzegn.html

[R09] 字符串比较
来源：http://hz.pycfn.com/gtqhziatbp.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.cdnleiting.top/gtwvufgsyl.html

[R10] 正则匹配
来源：http://hz.hysaishi.cn/gtgcpfbcgf.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.cucudq.cn/gtgadwtfvp.html

[R11] case 多分支
来源：http://hz.tianlin.xyz/gtklreteex.html

case "$1" in
来源：http://hz.jinqigfzy.top/gtzdslmikv.html

start) echo "启动" ;;
来源：http://hz.birdmap.top/gttdtiqgst.html

stop)  echo "停止" ;;
来源：http://hz.9152youxi.cn/gtrzeykzhp.html

*)     echo "未知命令" ;;
来源：http://hz.tianlin.xyz/gtcyeweqlv.html

esac
来源：http://hz.smart0.xyz/gtqileurph.html

[R12] for 遍历文件
来源：http://hz.nanxinkj.top/gtphgjlxyw.html

for f in *.txt; do echo "$f"; done
来源：http://hz.yvedp.cn/gtxqmpjjtd.html

[R13] for 计数循环
来源：http://hz.cqqwz.cn/gtaqaxniav.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.pengpengdd.cyou/gtdhxflmdu.html

[R14] C 风格 for
来源：http://hz.yueranfly.top/gtkahfeawf.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.snrcjt.cn/gtbntjxgoq.html

[R15] while 逐行读文件
来源：http://hz.cheryme.top/gtqyskfyyl.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.andypj.xyz/gtjxtyjiqs.html

[R16] until 等待条件
来源：http://hz.dianchejie.cn/gtfuhsbqtu.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.9152youxi.cn/gtidtxmyfr.html

[R17] 数组定义与取值
来源：http://hz.jlsjyb.cn/gtdggwnnzi.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.wangshuangyany.cn/gtfejrwzcn.html

[R18] 遍历数组
来源：http://hz.yuanzhike.top/gtuwqnkqwy.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.ehwqpu.com/gtvzmybomn.html

[R19] 数组长度
来源：http://hz.jinqigfzy.top/gtfsdzszdd.html

echo "${#arr[@]}"
来源：http://hz.yj20258.top/gtlhbpsktr.html

[R20] 关联数组（字典）
来源：http://hz.yj20258.top/gtpjhfmcbl.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.jinyuanbaomall.cn/gtksnfwfie.html

[R21] 字符串长度
来源：http://hz.meibo888.top/gtbauureko.html

echo "${#s}"
来源：http://hz.snrcjt.cn/gtajfcjyqq.html

[R22] 截取子串
来源：http://hz.ppjwa.cn/gtmitfilrf.html

echo "${s:0:5}"
来源：http://hz.0kj1m.cn/gtijatslli.html

[R23] 字符串替换
来源：http://hz.dashuyun.cn/gtuaqymfha.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.jyoumei.cn/gtyjljwxnc.html

[R24] 大小写转换
来源：http://hz.yanxiufei.cn/gtmeatqvhh.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.zhixingplan.top/gtlsnhnvpe.html

[R25] 去后缀 / 去前缀
来源：http://hz.nanxinkj.top/gtjwahviey.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.daxiang520.top/gtvxfxuovs.html

[R26] 命令替换
来源：http://hz.jlsjyb.cn/gtvwxshybr.html

now=$(date +%F); echo "$now"
来源：http://hz.jinqigfzy.top/gtmrxykbfy.html

[R27] 算术展开
来源：http://hz.nanxuanxn.top/gtpapdcpql.html

echo $((1 + 2 * 3))
来源：http://hz.havefunace.top/gtldwbfjjb.html

[R28] 浮点运算
来源：http://hz.mhx1999.top/gtxcvuflic.html

echo "scale=2; 10/3" | bc
来源：http://hz.ppjwa.cn/gttzudytql.html

[R29] 定义函数
来源：http://hz.hongshengwenyu.top/gteweqpugi.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.sufxvd.cn/gtvwxpabnb.html

[R30] 函数返回状态码
来源：http://hz.yueranfly.top/gtyltrtacu.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.yj20258888.top/gtgwvusttg.html

[R31] 局部变量
来源：http://hz.jqgufenzy.top/gthxibpmqc.html

f() { local x=1; echo "$x"; }
来源：http://hz.yueranfly.top/gtfltxusuv.html

[R32] 参数个数校验
来源：http://hz.ehwqpu.com/gtorctqodd.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.zhoulong.xyz/gtkxmqqhxk.html

[R33] 捕获错误并提示行号
来源：http://hz.ehwqpu.com/gtevvxbgka.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.nwbrower.top/gtltliwyjv.html

[R34] 退出时清理
来源：http://hz.ehwqpu.com/gtgcxqafla.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.zdqjudy.top/gtgzbhaitl.html

[R35] 后台执行并等待
来源：http://hz.hongshengwenyu.top/gtplczsgbk.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.hnqzz.top/gtknyzojeh.html

[R36] 并发执行多个任务
来源：http://hz.haohaochexian.top/gttiavvdxj.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.nanxinkj.top/gtcogvrlyw.html

[R37] 把输出赋给变量
来源：http://hz.ydjk.org.cn/gtlekqxxbb.html

files=$(ls -1)
来源：http://hz.ehwqpu.com/gtwlhonkha.html

[R38] 管道串联
来源：http://hz.zhengqikj.top/gtciqddwtw.html

cat a.txt | grep -i error | wc -l
来源：http://hz.haohaochexian.top/gturytvbyp.html

[R39] 重定向标准输出与错误
来源：http://hz.tianlin.xyz/gtdfdkghkt.html

cmd > out.log 2>&1
来源：http://hz.dashuyun.cn/gtginfkqbl.html

[R40] 追加写日志
来源：http://hz.c1oappe.top/gtohfphmib.html

echo "log" >> out.log
来源：http://hz.svipenyu.cn/gtzhudcbdi.html

[R41] 丢弃输出
来源：http://hz.cashguo.top/gtfjtqjymf.html

cmd >/dev/null 2>&1
来源：http://hz.shangyingyoupin.top/gtqhzltfra.html

[R42] 输入重定向
来源：http://hz.havefunace.top/gtrmlzqgaw.html

wc -l < a.txt
来源：http://hz.jlsjyb.cn/gtkfhetful.html

[R43] 按名字查找文件
来源：http://hz.52xcode.cn/gthbryejix.html

find . -name "*.log" -type f
来源：http://hz.aibaodan.cn/gtvwiwjwzg.html

[R44] 按修改时间查找
来源：http://hz.nanxinkj.top/gtsmaegwtm.html

find . -mtime -7 -type f
来源：http://hz.tanke756.top/gtxecrjuph.html

[R45] 批量删除
来源：http://hz.dashuyun.cn/gtjydmgzwb.html

find . -name "*.tmp" -delete
来源：http://hz.shanyushiyangkeji.top/gtxrspumao.html

[R46] 递归替换文件内容
来源：http://hz.smart0.xyz/gteuklycoc.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.shanyushiyangkeji.top/gthuogxsai.html

[R47] sed 单行替换
来源：http://hz.chenlongwang.top/gtxkcokxoj.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.yonumen.top/gtawisfonp.html

[R48] awk 取指定列
来源：http://hz.fengsongda.top/gtdwedekvk.html

awk '{print $1, $3}' a.txt
来源：http://hz.xingfuxueyuan.xyz/gtingaaqvq.html

[R49] awk 带条件
来源：http://hz.zdqjudy.top/gthmabgvng.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.birdmap.top/gtttxtnvaf.html

[R50] awk 求和
来源：http://hz.mhx1999.top/gtogaupgzi.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.sufxvd.cn/gtmspurrcw.html

[R51] 排序去重取前几
来源：http://hz.fzhhl.top/gtgpttvdwb.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.xinyue.icu/gtcknyhyzl.html

[R52] 统计行数
来源：http://hz.shuidangran.top/gtytzlyxhy.html

wc -l a.txt
来源：http://hz.ydjk.org.cn/gtpalxicpr.html

[R53] 查看文件头与实时尾
来源：http://hz.zhixingplan.top/gtvowjjymd.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.xziqi.cn/gtypztteyq.html

[R54] 比较两个文件
来源：http://hz.yangfankeji.com/gtyxzvhbkw.html

diff a.txt b.txt
来源：http://hz.aibaodan.cn/gthplhndvj.html

[R55] 压缩与解压
来源：http://hz.haohaochexian.top/gtbtdeqjwf.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.guowangkeji.top/gthcljdjug.html

[R56] 远程拷贝
来源：http://hz.cdnleiting.top/gtulomkbci.html

scp file user@host:/path/
来源：http://hz.ydjk.org.cn/gtjamomhmb.html

[R57] 远程执行命令
来源：http://hz.tanke756.top/gtswresnxw.html

ssh user@host 'uptime'
来源：http://hz.jiagoushi.top/gtzaostgue.html

[R58] 下载文件
来源：http://hz.zhengqikj.top/gtcqlfrnhk.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.hongshengwenyu.top/gtmpvjibek.html

[R59] 发 POST JSON
来源：http://hz.bjfxy.top/gtnipjqxwd.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.snrcjt.cn/gtybnrdzsw.html

[R60] 只看 HTTP 状态码
来源：http://hz.ehwqpu.com/gtuulqmrsx.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.jinqigufen.top/gtucmphfbu.html

[R61] 磁盘占用
来源：http://hz.cashguo.top/gtaxbnrxdz.html

df -h;  du -sh *
来源：http://hz.cashguo.top/gtrvsuvnhs.html

[R62] 找最占空间的文件
来源：http://hz.tanke756.top/gtlxagvmjw.html

du -ah . | sort -rh | head -10
来源：http://hz.jqgfzy.top/gtdnxzjqfu.html

[R63] 内存与进程
来源：http://hz.haohaochexian.top/gtrhdyugbl.html

free -h;  ps aux | grep nginx
来源：http://hz.bjfxy.top/gtckgolssb.html

[R64] 结束进程
来源：http://hz.ivvv.top/gtmbsiakrj.html

kill -9 $(pgrep -f app.py)
来源：http://hz.9152youxi.cn/gtfkidutat.html

[R65] 查看端口占用
来源：http://hz.havefunace.top/gtaeexmnze.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.mhx1999.top/gtjgjpogto.html

[R66] 定时任务
来源：http://hz.gogol.net.cn/gtsqagswzt.html

crontab -e;  crontab -l
来源：http://hz.shanyushiyangtech.top/gtoepqmfix.html

[R67] 生成随机十六进制串
来源：http://hz.chenzaomai.com/gtpygwbzrt.html

openssl rand -hex 16
来源：http://hz.hongshengwenyu.top/gthyfblodz.html

[R68] 计算文件校验值
来源：http://hz.jiagoushi.top/gtxccdzeyf.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.sysykeji.top/gtvufzxmqx.html

[R69] 生成随机密码
来源：http://hz.kuanghao11.cn/gtnkmquqnt.html

head -c 16 /dev/urandom | base64
来源：http://hz.cdnleiting.top/gtabgswval.html

[R70] 时间戳与互转
来源：http://hz.jlsjyb.cn/gtixlbtrwc.html

date +%s;  date -d @1700000000
来源：http://hz.shangyingyoupin.top/gtblotyrcm.html

[R71] 日期格式化
来源：http://hz.quarkkingdee.top/gtszirdfxn.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.chenlongwang.top/gtusgarnpz.html

[R72] 等待端口就绪
来源：http://hz.zhongyouzk.top/gtwjhwxaju.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.jyoumei.cn/gtttzgdrct.html

[R73] 分割大日志
来源：http://hz.meibo888.top/gtsckrmetx.html

split -l 1000 big.log part_
来源：http://hz.hammf.cn/gtppgmzinm.html

[R74] 批量重命名
来源：http://hz.52xcode.cn/gtkurhukpu.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.xinyue.icu/gtvtdacson.html

[R75] 导出环境变量
来源：http://hz.hongshengwenyu.top/gtrxbqmqxv.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.tian-w.cn/gttahyvash.html

[R76] 使用临时文件
来源：http://hz.sysykeji.top/gtxvrkslpg.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.guowangkeji.top/gtkbfreiwz.html

[R77] 读取用户输入
来源：http://hz.daxiang520.top/gtprkgyauj.html

read -rp "请输入: " ans
来源：http://hz.zhengqikj.top/gtyjweztcq.html

[R78] 交互式菜单
来源：http://hz.meibo888.top/gtgoawsknn.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.jqgfzy.top/gtfqowdxjp.html

[R79] 解析命令行选项
来源：http://hz.tanke756.top/gtzdirofcg.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.yangfankeji.com/gtkmwrqlnr.html

[R80] 查看脚本执行耗时
来源：http://hz.redwolf501.top/gtfdkllyca.html

time ./run.sh
来源：http://hz.sweek.top/gtphrjxbqx.html

================================================================================
来源：http://hz.yuanzhike.top/gtmkssxatq.html

S. C / C++ 专题
来源：http://hz.zhijiandao.cn/gtjsfdhqik.html

================================================================================
来源：http://hz.birdmap.top/gtmgdjiasq.html

[S01] C：Hello World
来源：http://hz.dashuyun.cn/gtotrcarak.html

#include <stdio.h>
来源：http://hz.cdnleiting.top/gtoxpoqsqu.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.ppjwa.cn/gtacvlvuwo.html

[S02] C：变量与格式化输出
来源：http://hz.yj20258888.top/gtubhjycqd.html

int a = 10; printf("%d\n", a);
来源：http://hz.zhaomingkeji.xyz/gtzoddjhyv.html

[S03] C：读入整数
来源：http://hz.zycfv.cn/gtrofsotqj.html

int x; scanf("%d", &x);
来源：http://hz.zycfv.cn/gtoftkduho.html

[S04] C：字符串复制
来源：http://hz.cdnleiting.top/gtycfeymoe.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.shangyingyoupin.top/gtduclzaew.html

[S05] C：字符串长度
来源：http://hz.zhoulong.xyz/gteecsstoa.html

strlen(s)
来源：http://hz.sysykeji.top/gtnannpnss.html

[S06] C：字符串比较
来源：http://hz.yangfankeji.com/gtqonruuza.html

strcmp(a, b) == 0
来源：http://hz.yvedp.cn/gtwsoxsqym.html

[S07] C：数组遍历求和
来源：http://hz.chenjidiqi.icu/gtzzdqygfy.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.daxiang520.top/gtucxpxvny.html

[S08] C：动态内存分配与释放
来源：http://hz.shanyushiyangtech.top/gtmehqmxvw.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.yueranfly.top/gtbgumwyei.html

[S09] C：结构体定义与初始化
来源：http://hz.redwolf501.top/gtwxqjshte.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.quarkkingdee.top/gtumcoeovd.html

[S10] C：指针与解引用
来源：http://hz.hysaishi.cn/gtbjwwqqdz.html

int *p = &a;  *p = 5;
来源：http://hz.havefunace.top/gterhsdfrr.html

[S11] C：逐行读文件
来源：http://hz.jqgfzy.top/gtkgeteona.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.cucudq.cn/gtmjctwpmd.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.fzhhl.top/gtajegxjuj.html

fclose(f);
来源：http://hz.gzhubu.top/gttwbgrfdp.html

[S12] C：写文件
来源：http://hz.guowangkeji.top/gtvcsxlmdn.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.zhixingplan.top/gtgkeauzfq.html

[S13] C：宏定义
来源：http://hz.sufxvd.cn/gtnjnvbzol.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.yuanzhike.top/gtdwxqmyer.html

[S14] C：枚举
来源：http://hz.hongshengwenyu.top/gtykipprqw.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.cdnleiting.top/gtxcxgligt.html

[S15] C：类型转换
来源：http://hz.52xcode.cn/gtnjzuovtc.html

(double) a / b
来源：http://hz.mhx1999.top/gtxiktfozt.html

[S16] C：位操作置位
来源：http://hz.iojbl.cn/gteufufyel.html

x |= (1 << 3);
来源：http://hz.yj202588.top/gtdqhtumnu.html

[S17] C：安全拼接字符串
来源：http://hz.yangfankeji.com/gtcjtsbsfc.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.shanyushiyangkeji.top/gtldrvyrbv.html

[S18] C：命令行参数
来源：http://hz.vqdsnc.cn/gtduxwuqtk.html

int main(int argc, char **argv)
来源：http://hz.zhengqikj.top/gtohcxxyby.html

[S19] C：快速排序
来源：http://hz.svipenyu.cn/gtjkyjjqdb.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.hammf.cn/gtuaihzxqd.html

[S20] C：二分查找
来源：http://hz.yj202588.top/gtyuyonrxz.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.chenlongwang.top/gtjsmhmidt.html

[S21] C：字符类别判断
来源：http://hz.tanke756.top/gtshzrwbid.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.bjfxy.top/gttnxiuxnj.html

[S22] C：字符串转数字
来源：http://hz.jinqigufen.top/gtwpqjjwky.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.jqgfzy.top/gtswbhbbav.html

[S23] C：随机数
来源：http://hz.gzhubu.top/gtwjwfgpyi.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.shangyingyoupin.top/gtqzhlajgs.html

[S24] C：获取本地时间
来源：http://hz.xingfuxueyuan.xyz/gtyqndrlmn.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.yueranfly.top/gtqsdducko.html

[S25] C：内存拷贝
来源：http://hz.mhx1999.top/gtjipuntkn.html

memcpy(dst, src, n);
来源：http://hz.gaohongyu789.top/gtzjycuzwo.html

[S26] C：内存清零
来源：http://hz.pengpengdd.cyou/gtqintmrmi.html

memset(a, 0, sizeof a);
来源：http://hz.cdnleiting.top/gtahwqolom.html

[S27] C：定义常量
来源：http://hz.yongpay.top/gtxejczztr.html

const double PI = 3.14159;
来源：http://hz.hammf.cn/gtbswxpkdt.html

[S28] C：静态变量
来源：http://hz.xinyue.icu/gthswpqusa.html

static int counter = 0;
来源：http://hz.hnqzz.top/gthsmvahyb.html

[S29] C：变参函数
来源：http://hz.gaohongyu789.top/gtbqdgjtqa.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.cdnleiting.top/gtbeklxmru.html

[S30] C：头文件保护
来源：http://hz.jyoumei.cn/gtlcxgfobq.html

#ifndef X_H
来源：http://hz.316326.xyz/gtzptvtmyf.html

#define X_H
来源：http://hz.ppjwa.cn/gtosqeyiox.html

#endif
来源：http://hz.jyoumei.cn/gtepetcdpx.html

[S31] C++：Hello World
来源：http://hz.jqgfzy.top/gtzbwyhamo.html

#include <iostream>
来源：http://hz.ehwqpu.com/gtwzkhfqkx.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.quarkkingdee.top/gtkfxttxro.html

[S32] C++：字符串
来源：http://hz.zhijiandao.cn/gtincogmbf.html

std::string s = "hi";  s += "!";
来源：http://hz.yj202588.top/gtvtqfdddb.html

[S33] C++：vector 增删
来源：http://hz.dianchejie.cn/gttcvetglw.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.gzhubu.top/gtqalhdcxm.html

[S34] C++：遍历 vector
来源：http://hz.andypj.xyz/gtqwghiuus.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.daxiang520.top/gtnnaemtpz.html

[S35] C++：map
来源：http://hz.zhengqikj.top/gthgnjfdjm.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.hfpthk.cn/gtzylcrfif.html

[S36] C++：unordered_map
来源：http://hz.shanyushiyangtech.top/gteudhpomr.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.zhijiandao.cn/gtrxywgmti.html

[S37] C++：set
来源：http://hz.0kj1m.cn/gtpymhkwwf.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.ydzc1.top/gttyibpgxe.html

[S38] C++：排序
来源：http://hz.jqgfzy.top/gtkoiqbcvk.html

std::sort(v.begin(), v.end());
来源：http://hz.jiagoushi.top/gtwadbmper.html

[S39] C++：自定义比较器排序
来源：http://hz.316326.xyz/gtosqrldus.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.gotoacloud.top/gtqzanwlyd.html

[S40] C++：查找元素
来源：http://hz.zhiwuduotai.top/gtycstdfzn.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.shanyushiyangtech.top/gttajopqtn.html

[S41] C++：类与构造函数
来源：http://hz.hnqzz.top/gtdcckuwcn.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.pengpengdd.cyou/gtxeinblmx.html

[S42] C++：继承与虚函数
来源：http://hz.jianghu66.top/gtmuvqtqvf.html

class B : public Base { public: void f() override {} };
来源：http://hz.shanyushiyangtech.top/gtcfnqzmdx.html

[S43] C++：智能指针
来源：http://hz.ppjwa.cn/gtydgpelpy.html

auto p = std::make_unique<int>(5);
来源：http://hz.gotoacloud.top/gtpdhhtmwz.html

[S44] C++：引用传参
来源：http://hz.9152youxi.cn/gtpokhlkxr.html

void inc(int &x) { ++x; }
来源：http://hz.fengsongda.top/gtqcorpwjl.html

[S45] C++：lambda
来源：http://hz.xziqi.cn/gtqgwurhki.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.zhaomingkeji.xyz/gtossmggee.html

[S46] C++：函数模板
来源：http://hz.jyoumei.cn/gtzkfqqjxo.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.gotoacloud.top/gthouhyhln.html

[S47] C++：结构化绑定遍历
来源：http://hz.iojbl.cn/gtuujhkdtp.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.andypj.xyz/gtsgmywevc.html

[S48] C++：逐行读文件
来源：http://hz.aibaodan.cn/gtdixuzwde.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.yj20258.top/gtysfmdasy.html


<!-- 参考信息 -->