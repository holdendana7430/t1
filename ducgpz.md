代发 wailian999

SHOW INDEX FROM users;
来源：http://hz.yongpay.top/gtdkzszbgx.html

[Q73] 查看表状态
来源：http://hz.ppjwa.cn/gtlfthjdym.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.hnxiangtu.top/gtdxitpilg.html

[Q74] 强制使用索引
来源：http://hz.aizwys.cn/gtdhgrdten.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.hnqzz.top/gtgzfvwcnq.html

[Q75] 日期格式化
来源：http://hz.zhoulong.xyz/gtwocsciqx.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.chenzaomai.com/gtbeboeiyf.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.yonumen.top/gtiivhusmq.html

[Q76] 按天统计
来源：http://hz.gotoacloud.top/gtwhmsvtsl.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.xinyue.icu/gtogiyexmn.html

[Q77] 时间加减
来源：http://hz.shanyushiyangtech.top/gtoqukxuon.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.kuanghao11.cn/gtrvvoseck.html

[Q78] 当前时间
来源：http://hz.vqdsnc.cn/gtsrpuaprq.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.zhijiandao.cn/gtnyiknbpr.html

[Q79] 字符串拼接
来源：http://hz.ppjwa.cn/gtukfiskzd.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.dianchejie.cn/gtpolcjwxo.html

[Q80] 字符串截取
来源：http://hz.gogol.net.cn/gtidoawuvo.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.tian-w.cn/gtdbfnmmdk.html

[Q81] 字符串替换
来源：http://hz.zhixingplan.top/gtuyzgthxm.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.daria6918.cn/gtbusdllng.html

[Q82] 字符长度与字节长度
来源：http://hz.tianlin.xyz/gtdioitouv.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.chenlongwang.top/gthpcjyrxo.html

[Q83] 大小写转换
来源：http://hz.jqgufenzy.top/gttryozghh.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.yongpay.top/gtbxgkzixk.html

[Q84] 去除首尾空格
来源：http://hz.gotoacloud.top/gtsmicunre.html

SELECT TRIM(name) FROM users;
来源：http://hz.316326.xyz/gtaxjcdnsa.html

[Q85] 数值取整
来源：http://hz.hysaishi.cn/gtlnrhkfdw.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.nwbrower.top/gtsheucxri.html

[Q86] 读取 JSON 字段
来源：http://hz.cucudq.cn/gtkdzqcrzj.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.bjfxy.top/gtshhvmvzu.html

[Q87] JSON 字段做条件
来源：http://hz.hywenlv.cn/gtlbrqhfib.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.dashuyun.cn/gtknygnmuq.html

[Q88] 行转列（条件聚合）
来源：http://hz.zhoulong.xyz/gtmwvydpwv.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.jinqigufen.top/gtaikecelm.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.0kj1m.cn/gtrioqhopj.html

[Q89] 判断表是否存在
来源：http://hz.ivvv.top/gtqmzvicah.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.nwbrower.top/gtqsmonsev.html

[Q90] 生成序号列
来源：http://hz.c1oappe.top/gtdwuendgy.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.birdmap.top/gtzsgwxvol.html

================================================================================
来源：http://hz.zhengqikj.top/gtozrdcaaf.html

R. Bash 专题
来源：http://hz.nwbrower.top/gtckrlzcop.html

================================================================================
来源：http://hz.kuanghao11.cn/gtmprnkanz.html

[R01] shebang 与严格模式
来源：http://hz.shangyingyoupin.top/gtrxvkqtoj.html

#!/usr/bin/env bash
来源：http://hz.kuanghao11.cn/gtzgfefmgf.html

set -euo pipefail
来源：http://hz.iojbl.cn/gthstytrxt.html

[R02] 变量赋值与使用
来源：http://hz.zhijiandao.cn/gtizufujal.html

name="Tom"; echo "$name"
来源：http://hz.chenzaomai.com/gtmvuasfmv.html

[R03] 只读变量
来源：http://hz.nanxinkj.top/gtiankutpr.html

readonly PI=3.14
来源：http://hz.sweek.top/gtwsgvkhxj.html

[R04] 位置参数
来源：http://hz.hysaishi.cn/gtxrkwoqzb.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.hysaishi.cn/gtwghtoxtm.html

[R05] 参数默认值
来源：http://hz.cdnleiting.top/gticwytdaz.html

name="${1:-default}"
来源：http://hz.xingfuxueyuan.xyz/gtwxcnguxa.html

[R06] 判断命令是否存在
来源：http://hz.vqdsnc.cn/gtecvwdnmf.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.nanxinkj.top/gtnpzjkmxd.html

[R07] if 判断文件
来源：http://hz.yj20258888.top/gtradnikbl.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.smart0.xyz/gttkotvdif.html

[R08] 数值比较
来源：http://hz.birdmap.top/gthgjeotqm.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.yonumen.top/gtztvtsnmw.html

[R09] 字符串比较
来源：http://hz.mhx1999.top/gtspreegev.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.redwolf501.top/gtqbnzcjmn.html

[R10] 正则匹配
来源：http://hz.pengpengdd.cyou/gtydlxeaya.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.jiagoushi.top/gtqbwdyizi.html

[R11] case 多分支
来源：http://hz.shuidangran.top/gtnfsmwctr.html

case "$1" in
来源：http://hz.svipenyu.cn/gtvblokkav.html

start) echo "启动" ;;
来源：http://hz.havefunace.top/gtwumwgyqc.html

stop)  echo "停止" ;;
来源：http://hz.yj20258888.top/gtlqdhzfbm.html

*)     echo "未知命令" ;;
来源：http://hz.zhiwuduotai.top/gtzclkqedh.html

esac
来源：http://hz.zhijiandao.cn/gtidpomaoj.html

[R12] for 遍历文件
来源：http://hz.hywenlv.cn/gttuwmlppr.html

for f in *.txt; do echo "$f"; done
来源：http://hz.xuanzx.com/gtkzpgfnpw.html

[R13] for 计数循环
来源：http://hz.yj202588.top/gthidtyfks.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.pengpengdd.cyou/gtntsoogyf.html

[R14] C 风格 for
来源：http://hz.jianghu66.top/gtfpuabqit.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.ppjwa.cn/gtmxrqvzyq.html

[R15] while 逐行读文件
来源：http://hz.gotoacloud.top/gtaysoybje.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.jinqigufen.top/gtslqgsdee.html

[R16] until 等待条件
来源：http://hz.zycfv.cn/gtiepordpv.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.tanke756.top/gtnxbdbjle.html

[R17] 数组定义与取值
来源：http://hz.tian-w.cn/gtbzemideb.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.smart0.xyz/gtpvfghvid.html

[R18] 遍历数组
来源：http://hz.fengsongda.top/gtlhvemjww.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.snrcjt.cn/gtbjswsgzh.html

[R19] 数组长度
来源：http://hz.hysaishi.cn/gtxkknkkye.html

echo "${#arr[@]}"
来源：http://hz.bjfxy.top/gtxdwycbwr.html

[R20] 关联数组（字典）
来源：http://hz.xuanzx.com/gtmbfsskmd.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.yj20258.top/gtjxppebtm.html

[R21] 字符串长度
来源：http://hz.cashguo.top/gthljwgvaf.html

echo "${#s}"
来源：http://hz.zhoulong.xyz/gtqumnuams.html

[R22] 截取子串
来源：http://hz.vqdsnc.cn/gtuawlcick.html

echo "${s:0:5}"
来源：http://hz.gogol.net.cn/gtzokwjnsb.html

[R23] 字符串替换
来源：http://hz.zhixingplan.top/gtqpwihjlq.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.dashuyun.cn/gtlthvjlep.html

[R24] 大小写转换
来源：http://hz.zycfv.cn/gtasvlizbv.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.0kj1m.cn/gtjzvegqtb.html

[R25] 去后缀 / 去前缀
来源：http://hz.guannengcc.top/gtybwjjowy.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.cheryme.top/gtmcyzwxdq.html

[R26] 命令替换
来源：http://hz.shzxlz.cn/gtoprxcdtp.html

now=$(date +%F); echo "$now"
来源：http://hz.daxiang520.top/gtrtshplqt.html

[R27] 算术展开
来源：http://hz.zhiwuduotai.top/gtkwwytazk.html

echo $((1 + 2 * 3))
来源：http://hz.shanyushiyangtech.top/gtxfegbiqn.html

[R28] 浮点运算
来源：http://hz.zhixingplan.top/gtgycsmdfe.html

echo "scale=2; 10/3" | bc
来源：http://hz.feifeiyinyue.top/gtsxmsdedj.html

[R29] 定义函数
来源：http://hz.yuxming.cn/gtkjdggocy.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.zhixingplan.top/gtchinzzqu.html

[R30] 函数返回状态码
来源：http://hz.hnxiangtu.top/gtfhaloitm.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.hysaishi.cn/gttjxjuwxp.html

[R31] 局部变量
来源：http://hz.52xcode.cn/gtdlyiyzma.html

f() { local x=1; echo "$x"; }
来源：http://hz.shzxlz.cn/gtjnygqkfs.html

[R32] 参数个数校验
来源：http://hz.zhixingplan.top/gtdcvszoeu.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.jqgufenzy.top/gtntjtajip.html

[R33] 捕获错误并提示行号
来源：http://hz.wangshuangyany.cn/gtcfcgfhwj.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.ehwqpu.com/gtqxnqltry.html

[R34] 退出时清理
来源：http://hz.yj202588.top/gtvwtohxeu.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.smart0.xyz/gtfbcttuti.html

[R35] 后台执行并等待
来源：http://hz.hysaishi.cn/gtazgetcba.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.jqgfzy.top/gtvwyzwgjw.html

[R36] 并发执行多个任务
来源：http://hz.hysaishi.cn/gtqcgruuau.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.shanyushiyangtech.top/gtositojxn.html

[R37] 把输出赋给变量
来源：http://hz.dashuyun.cn/gtsleidjex.html

files=$(ls -1)
来源：http://hz.yanxiufei.cn/gtexudfkju.html

[R38] 管道串联
来源：http://hz.sweek.top/gtjgtrmbls.html

cat a.txt | grep -i error | wc -l
来源：http://hz.jianghu66.top/gtisaaxcpo.html

[R39] 重定向标准输出与错误
来源：http://hz.zhiwuduotai.top/gtburlahaq.html

cmd > out.log 2>&1
来源：http://hz.hfpthk.cn/gtrbdageun.html

[R40] 追加写日志
来源：http://hz.shangyingyoupin.top/gtzyjikmqh.html

echo "log" >> out.log
来源：http://hz.zhengqikj.top/gtolyzdpkm.html

[R41] 丢弃输出
来源：http://hz.vqdsnc.cn/gtueeltshx.html

cmd >/dev/null 2>&1
来源：http://hz.zhaomingkeji.xyz/gthrbbcvts.html

[R42] 输入重定向
来源：http://hz.hammf.cn/gtzpgcjdto.html

wc -l < a.txt
来源：http://hz.jqgufenzy.top/gtvkanvmhz.html

[R43] 按名字查找文件
来源：http://hz.daria6918.cn/gtkvhtzqhc.html

find . -name "*.log" -type f
来源：http://hz.xingfuxueyuan.xyz/gtbpyqfctk.html

[R44] 按修改时间查找
来源：http://hz.meibo888.top/gtlssrtebs.html

find . -mtime -7 -type f
来源：http://hz.shanyushiyangkeji.top/gtsiwcdhkx.html

[R45] 批量删除
来源：http://hz.jqgufenzy.top/gtnicykktx.html

find . -name "*.tmp" -delete
来源：http://hz.daria6918.cn/gtkqgbuizh.html

[R46] 递归替换文件内容
来源：http://hz.daria6918.cn/gthhzdency.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.cucudq.cn/gtjhewljim.html

[R47] sed 单行替换
来源：http://hz.ehwqpu.com/gtbbhsprrz.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.ivvv.top/gtfrsdkgef.html

[R48] awk 取指定列
来源：http://hz.fzhhl.top/gtzpisgfru.html

awk '{print $1, $3}' a.txt
来源：http://hz.yonumen.top/gtpxhreemj.html

[R49] awk 带条件
来源：http://hz.dianchejie.cn/gtxgolaext.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.zhongyouzk.top/gtgvkvepdb.html

[R50] awk 求和
来源：http://hz.cheryme.top/gtyxrltdao.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.feifeiyinyue.top/gtllieltdx.html

[R51] 排序去重取前几
来源：http://hz.shzxlz.cn/gtqgzdftar.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.ehwqpu.com/gtqvstbqro.html

[R52] 统计行数
来源：http://hz.zhixingplan.top/gtnavwftxe.html

wc -l a.txt
来源：http://hz.yongpay.top/gtnwzxcyla.html

[R53] 查看文件头与实时尾
来源：http://hz.sysykeji.top/gtkuhmkkhq.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.0kj1m.cn/gtaponajxk.html

[R54] 比较两个文件
来源：http://hz.yvedp.cn/gtpjtyhwhb.html

diff a.txt b.txt
来源：http://hz.wangdashe.top/gtucaambcl.html

[R55] 压缩与解压
来源：http://hz.zhengqikj.top/gtvuninzih.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.hywenlv.cn/gtgpvfymts.html

[R56] 远程拷贝
来源：http://hz.zdqjudy.top/gtxkosiyxf.html

scp file user@host:/path/
来源：http://hz.yj20258.top/gtoscfwjyf.html

[R57] 远程执行命令
来源：http://hz.shangyingyoupin.top/gtojnnxsuy.html

ssh user@host 'uptime'
来源：http://hz.nanxuanxn.top/gtafnakdyt.html

[R58] 下载文件
来源：http://hz.yueranfly.top/gtelvimwrn.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.52xcode.cn/gthcwqqefs.html

[R59] 发 POST JSON
来源：http://hz.cashguo.top/gtsxezqoze.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.guowangkeji.top/gtwkrpafne.html

[R60] 只看 HTTP 状态码
来源：http://hz.fengsongda.top/gtsfadcbgf.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.pengpengdd.cyou/gtnsopfuwo.html

[R61] 磁盘占用
来源：http://hz.yvedp.cn/gtwncwdllv.html

df -h;  du -sh *
来源：http://hz.jinqigfzy.top/gtpiqpmqfb.html

[R62] 找最占空间的文件
来源：http://hz.zhengqikj.top/gttnkrammn.html

du -ah . | sort -rh | head -10
来源：http://hz.pycfn.com/gtiyoqruwe.html

[R63] 内存与进程
来源：http://hz.cucudq.cn/gtlxttatsf.html

free -h;  ps aux | grep nginx
来源：http://hz.yangfankeji.com/gtvwidqynh.html

[R64] 结束进程
来源：http://hz.yuxming.cn/gtrnmwkpfb.html

kill -9 $(pgrep -f app.py)
来源：http://hz.ehwqpu.com/gtjtkabzei.html

[R65] 查看端口占用
来源：http://hz.havefunace.top/gtayuayahi.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.zhijiandao.cn/gtzzmjhmmg.html

[R66] 定时任务
来源：http://hz.bjfxy.top/gtzisrwlyw.html

crontab -e;  crontab -l
来源：http://hz.tanke756.top/gtveyfimkt.html

[R67] 生成随机十六进制串
来源：http://hz.birdmap.top/gtidtavegt.html

openssl rand -hex 16
来源：http://hz.dashuyun.cn/gtqpyianjr.html

[R68] 计算文件校验值
来源：http://hz.ppjwa.cn/gtdabevrbw.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.yanxiufei.cn/gtjptynyay.html

[R69] 生成随机密码
来源：http://hz.smart0.xyz/gtvdpgakfu.html

head -c 16 /dev/urandom | base64
来源：http://hz.ydzc1.top/gtdkalwxbv.html

[R70] 时间戳与互转
来源：http://hz.ppjwa.cn/gtvfdjvokd.html

date +%s;  date -d @1700000000
来源：http://hz.xylfe.cn/gtjwgyujez.html

[R71] 日期格式化
来源：http://hz.hysaishi.cn/gtvrzwdjxb.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.zycfv.cn/gtlxliynyh.html

[R72] 等待端口就绪
来源：http://hz.yanxiufei.cn/gtmtqgpwtq.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.zhiwuduotai.top/gtmspgiajf.html

[R73] 分割大日志
来源：http://hz.zhiwuduotai.top/gtambclntv.html

split -l 1000 big.log part_
来源：http://hz.jinghuilouyu.cn/gtcecsnisu.html

[R74] 批量重命名
来源：http://hz.cdnleiting.top/gtthfsnjqk.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.hysaishi.cn/gtyzbmqfis.html

[R75] 导出环境变量
来源：http://hz.ehwqpu.com/gtxrqzhxwi.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.hammf.cn/gtgmljzuyw.html

[R76] 使用临时文件
来源：http://hz.guowangkeji.top/gtgrmzyhyl.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.yongpay.top/gtpyoqxaes.html

[R77] 读取用户输入
来源：http://hz.andypj.xyz/gtlbubouiq.html

read -rp "请输入: " ans
来源：http://hz.chenlongwang.top/gtohcemnvk.html

[R78] 交互式菜单
来源：http://hz.yueranfly.top/gtdtjmeani.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.hysaishi.cn/gtfuwydvmw.html

[R79] 解析命令行选项
来源：http://hz.316326.xyz/gtbazggttj.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.cashguo.top/gtmemdhqdq.html

[R80] 查看脚本执行耗时
来源：http://hz.jiagoushi.top/gtxweomebn.html

time ./run.sh
来源：http://hz.hywenlv.cn/gtdrqltsrh.html

================================================================================
来源：http://hz.bjfxy.top/gttuumdivq.html

S. C / C++ 专题
来源：http://hz.hysaishi.cn/gtqxtelgzy.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtikggmwox.html

[S01] C：Hello World
来源：http://hz.mhx1999.top/gteabkszzj.html

#include <stdio.h>
来源：http://hz.dianchejie.cn/gtwtxjcaec.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.zhaomingkeji.xyz/gtfwqlkrxt.html

[S02] C：变量与格式化输出
来源：http://hz.cdnleiting.top/gttvovmwyv.html

int a = 10; printf("%d\n", a);
来源：http://hz.hnxiangtu.top/gtwvdufoab.html

[S03] C：读入整数
来源：http://hz.zhiwuduotai.top/gtpceobsgd.html

int x; scanf("%d", &x);
来源：http://hz.bjfxy.top/gtokdjgovn.html

[S04] C：字符串复制
来源：http://hz.birdmap.top/gtkmfhgoez.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.yj20258888.top/gtumdobfae.html

[S05] C：字符串长度
来源：http://hz.snrcjt.cn/gtyxitrzie.html

strlen(s)
来源：http://hz.nwbrower.top/gtycyyqevr.html

[S06] C：字符串比较
来源：http://hz.svipenyu.cn/gtmuluceey.html

strcmp(a, b) == 0
来源：http://hz.9152youxi.cn/gtrryaxbtb.html

[S07] C：数组遍历求和
来源：http://hz.tanke756.top/gttsyepbby.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.aibaodan.cn/gtcyjbpleb.html

[S08] C：动态内存分配与释放
来源：http://hz.zdqjudy.top/gtmnqgxhzl.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.shangyingyoupin.top/gtzrvgsyaq.html

[S09] C：结构体定义与初始化
来源：http://hz.yueranfly.top/gtsywwwpij.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.jinyuanbaomall.cn/gthekyelhe.html

[S10] C：指针与解引用
来源：http://hz.bjfxy.top/gtmrilmfty.html

int *p = &a;  *p = 5;
来源：http://hz.jiagoushi.top/gtcgwqvntn.html

[S11] C：逐行读文件
来源：http://hz.yueranfly.top/gtsfwusqof.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.xuetiantiany.cn/gtyqttqrqh.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.dashuyun.cn/gtupadjjcp.html

fclose(f);
来源：http://hz.jinyuanbaomall.cn/gtaojbupgo.html

[S12] C：写文件
来源：http://hz.xinyue.icu/gtbugcddmq.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.zhaomingkeji.xyz/gtwefajtvi.html

[S13] C：宏定义
来源：http://hz.jinqigufen.top/gtwdspgxix.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.dianchejie.cn/gtongkhoni.html

[S14] C：枚举
来源：http://hz.zhengqikj.top/gtbjfhiwll.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.cheryme.top/gtbokefrut.html

[S15] C：类型转换
来源：http://hz.yonumen.top/gtfxihtspn.html

(double) a / b
来源：http://hz.vqdsnc.cn/gtyzizkwji.html

[S16] C：位操作置位
来源：http://hz.daria6918.cn/gtusgynqpk.html

x |= (1 << 3);
来源：http://hz.aibaodan.cn/gtvvuocqpd.html

[S17] C：安全拼接字符串
来源：http://hz.gaohongyu789.top/gtolruksue.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.yanxiufei.cn/gtwcmnjkwx.html

[S18] C：命令行参数
来源：http://hz.cdnleiting.top/gtzcryxaam.html

int main(int argc, char **argv)
来源：http://hz.iojbl.cn/gtvkbmhmpo.html

[S19] C：快速排序
来源：http://hz.shanyushiyangkeji.top/gtmlqhkvut.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.dianchejie.cn/gtonwqdutw.html

[S20] C：二分查找
来源：http://hz.nanxinkj.top/gtrzihaijd.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.shangyingyoupin.top/gtanrpudja.html

[S21] C：字符类别判断
来源：http://hz.hongshengwenyu.top/gtcuzzzbmp.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.ppjwa.cn/gteymgcbjs.html

[S22] C：字符串转数字
来源：http://hz.tanke756.top/gtrxpjrpnv.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.mhx1999.top/gtmfndodrv.html

[S23] C：随机数
来源：http://hz.hysaishi.cn/gtqlohvtbz.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.iojbl.cn/gtvbkfvkzx.html

[S24] C：获取本地时间
来源：http://hz.zhoulong.xyz/gtdwwtgqdv.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.hammf.cn/gtciprnrtm.html

[S25] C：内存拷贝
来源：http://hz.hongshengwenyu.top/gtddotallh.html

memcpy(dst, src, n);
来源：http://hz.mhx1999.top/gtmqotglts.html

[S26] C：内存清零
来源：http://hz.haohaochexian.top/gtwtrbuaqd.html

memset(a, 0, sizeof a);
来源：http://hz.zhixingplan.top/gtjsikpnhc.html

[S27] C：定义常量
来源：http://hz.yj20258888.top/gtkhqczydj.html

const double PI = 3.14159;
来源：http://hz.gzhubu.top/gtuinsdofi.html

[S28] C：静态变量
来源：http://hz.yuxming.cn/gtglxhwwca.html

static int counter = 0;
来源：http://hz.zhixingplan.top/gtgkpsaijw.html

[S29] C：变参函数
来源：http://hz.jiagoushi.top/gtqctmlxei.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.cdnleiting.top/gtufxipzog.html

[S30] C：头文件保护
来源：http://hz.yuxming.cn/gtpzetkvgp.html

#ifndef X_H
来源：http://hz.xziqi.cn/gtqqkgzyrk.html

#define X_H
来源：http://hz.haohaochexian.top/gtlbfbxmcm.html

#endif
来源：http://hz.zhaomingkeji.xyz/gtvzssmiup.html

[S31] C++：Hello World
来源：http://hz.wangshuangyany.cn/gtkmkkloyk.html

#include <iostream>
来源：http://hz.xziqi.cn/gtywiusswx.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.yuxming.cn/gtljpyywiw.html

[S32] C++：字符串
来源：http://hz.hongshengwenyu.top/gtzuuownnu.html

std::string s = "hi";  s += "!";
来源：http://hz.jiagoushi.top/gtlraefxlt.html

[S33] C++：vector 增删
来源：http://hz.zhiwuduotai.top/gtrelifvig.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.ybcxt.top/gtfnvfqkzs.html

[S34] C++：遍历 vector
来源：http://hz.sysykeji.top/gtokvuruzp.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.gaohongyu789.top/gtqwiiznpz.html

[S35] C++：map
来源：http://hz.dianchejie.cn/gthleruhyv.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.sweek.top/gtxogxaubb.html

[S36] C++：unordered_map
来源：http://hz.xylfe.cn/gtpgfnyijw.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.pycfn.com/gtdexwezch.html

[S37] C++：set
来源：http://hz.cucudq.cn/gtuiuhinvv.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.wangshuangyany.cn/gtwppnwkxb.html

[S38] C++：排序
来源：http://hz.bjfxy.top/gtpjyeobix.html

std::sort(v.begin(), v.end());
来源：http://hz.ydjk.org.cn/gtwstzztvr.html

[S39] C++：自定义比较器排序
来源：http://hz.zhongyouzk.top/gtydymymny.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.xuetiantiany.cn/gtqeyuxgoe.html

[S40] C++：查找元素
来源：http://hz.yongpay.top/gtprkjvmrn.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.shanyushiyangtech.top/gtescxpaxv.html

[S41] C++：类与构造函数
来源：http://hz.zhongyouzk.top/gtiwnfemfg.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.zhongyouzk.top/gtffczufks.html

[S42] C++：继承与虚函数
来源：http://hz.hysaishi.cn/gthbvtbiey.html

class B : public Base { public: void f() override {} };
来源：http://hz.ywan-chungtsiang.top/gtewbwufmn.html


<!-- 参考信息 -->