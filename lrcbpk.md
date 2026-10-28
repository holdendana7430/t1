代发 wailian999

[Q76] 按天统计
来源：http://hz.jinqigfzy.top/gtgpuurmeg.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.ppjwa.cn/gtayhwelxr.html

[Q77] 时间加减
来源：http://hz.shzxlz.cn/gtboceeqrf.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.gzhubu.top/gtesmycerm.html

[Q78] 当前时间
来源：http://hz.ybcxt.top/gthpjhfzcr.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.pycfn.com/gtaqqoptpq.html

[Q79] 字符串拼接
来源：http://hz.cucudq.cn/gtrcuvpliy.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.ppjwa.cn/gtwktiksii.html

[Q80] 字符串截取
来源：http://hz.jinghuilouyu.cn/gtzszytgxx.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.svipenyu.cn/gtgaoledsk.html

[Q81] 字符串替换
来源：http://hz.bjfxy.top/gtbwmuyduo.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.tianlin.xyz/gtajecbcit.html

[Q82] 字符长度与字节长度
来源：http://hz.xinyue.icu/gtnpvnelnq.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.yvedp.cn/gtvxgrrlpk.html

[Q83] 大小写转换
来源：http://hz.jqgufenzy.top/gthdjrwqde.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.aibaodan.cn/gtmubyhnmw.html

[Q84] 去除首尾空格
来源：http://hz.dianchejie.cn/gtrhzozyzg.html

SELECT TRIM(name) FROM users;
来源：http://hz.haohaochexian.top/gtvowbycrn.html

[Q85] 数值取整
来源：http://hz.gzhubu.top/gtamlctwux.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.xuetiantiany.cn/gtuqygmqym.html

[Q86] 读取 JSON 字段
来源：http://hz.xinyue.icu/gtvwfthqlx.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.yangfankeji.com/gtlfzqgmnq.html

[Q87] JSON 字段做条件
来源：http://hz.cashguo.top/gtwlbxqqdc.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.jinqigufen.top/gtvwwtsodc.html

[Q88] 行转列（条件聚合）
来源：http://hz.zhongyouzk.top/gtyfyfemqw.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.guannengcc.top/gtdrhrahka.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.xingfuxueyuan.xyz/gtevtgbnrv.html

[Q89] 判断表是否存在
来源：http://hz.xylfe.cn/gtjihqxqht.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.iojbl.cn/gtzorcklwl.html

[Q90] 生成序号列
来源：http://hz.cashguo.top/gtrrnvtlen.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.jianghu66.top/gtbbslbxso.html

================================================================================
来源：http://hz.yonumen.top/gttepilyhd.html

R. Bash 专题
来源：http://hz.quarkkingdee.top/gtqynyxbgn.html

================================================================================
来源：http://hz.aizwys.cn/gtwizimymq.html

[R01] shebang 与严格模式
来源：http://hz.yvedp.cn/gtsgyrgtod.html

#!/usr/bin/env bash
来源：http://hz.jiagoushi.top/gtyfrvmrsq.html

set -euo pipefail
来源：http://hz.shuidangran.top/gtkkgjckha.html

[R02] 变量赋值与使用
来源：http://hz.havefunace.top/gteaqkwvcn.html

name="Tom"; echo "$name"
来源：http://hz.gotoacloud.top/gtztmwqajo.html

[R03] 只读变量
来源：http://hz.guannengcc.top/gtbjxbzxsr.html

readonly PI=3.14
来源：http://hz.snrcjt.cn/gtdjwtoeuo.html

[R04] 位置参数
来源：http://hz.hysaishi.cn/gtyoguxsyp.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.fengsongda.top/gtefchqtoy.html

[R05] 参数默认值
来源：http://hz.jyoumei.cn/gtyixdwqii.html

name="${1:-default}"
来源：http://hz.feifeiyinyue.top/gtqfsjvqrf.html

[R06] 判断命令是否存在
来源：http://hz.cdnleiting.top/gthlmoijax.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.fzhhl.top/gteravpyiz.html

[R07] if 判断文件
来源：http://hz.nwbrower.top/gtretydcaz.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.sufxvd.cn/gterrmjbxk.html

[R08] 数值比较
来源：http://hz.redwolf501.top/gtwsyarrbc.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.xinyue.icu/gtiuywbyps.html

[R09] 字符串比较
来源：http://hz.birdmap.top/gtucqrxupk.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.redwolf501.top/gttldlsgmr.html

[R10] 正则匹配
来源：http://hz.yongpay.top/gtbjmxkphn.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.hnqzz.top/gttkpcwmxs.html

[R11] case 多分支
来源：http://hz.hongshengwenyu.top/gttaxuaefp.html

case "$1" in
来源：http://hz.xingfuxueyuan.xyz/gtpggizdpg.html

start) echo "启动" ;;
来源：http://hz.fengsongda.top/gttnguztbk.html

stop)  echo "停止" ;;
来源：http://hz.daria6918.cn/gtyqihrqgu.html

*)     echo "未知命令" ;;
来源：http://hz.aizwys.cn/gtrsburwhj.html

esac
来源：http://hz.hfpthk.cn/gtitdiujzv.html

[R12] for 遍历文件
来源：http://hz.ydjk.org.cn/gtgwixkojk.html

for f in *.txt; do echo "$f"; done
来源：http://hz.havefunace.top/gtackmnvty.html

[R13] for 计数循环
来源：http://hz.meibo888.top/gthgmkobry.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.cashguo.top/gtehjjoxds.html

[R14] C 风格 for
来源：http://hz.bjfxy.top/gthwmcgtwt.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.gzhubu.top/gtfkvmvvma.html

[R15] while 逐行读文件
来源：http://hz.cqqwz.cn/gtjslspaux.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.tanke756.top/gtdeiinpkc.html

[R16] until 等待条件
来源：http://hz.feifeiyinyue.top/gtousizshk.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.havefunace.top/gtyodntcsw.html

[R17] 数组定义与取值
来源：http://hz.wangdashe.top/gtcafjgnac.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.svipenyu.cn/gtiyeeodmw.html

[R18] 遍历数组
来源：http://hz.hywenlv.cn/gtskdzygdp.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.hongshengwenyu.top/gtvydnxjbz.html

[R19] 数组长度
来源：http://hz.yonumen.top/gtbqdpaipg.html

echo "${#arr[@]}"
来源：http://hz.mhx1999.top/gtflnsptsc.html

[R20] 关联数组（字典）
来源：http://hz.jinqigufen.top/gtlymkssya.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.zycfv.cn/gtpukwjiyl.html

[R21] 字符串长度
来源：http://hz.yvedp.cn/gtbgufzkrf.html

echo "${#s}"
来源：http://hz.xuanzx.com/gtinpmqyhr.html

[R22] 截取子串
来源：http://hz.andypj.xyz/gtnuexcmth.html

echo "${s:0:5}"
来源：http://hz.wangshuangyany.cn/gtptnxcixt.html

[R23] 字符串替换
来源：http://hz.redwolf501.top/gtdepngzgr.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.ivvv.top/gteueubzet.html

[R24] 大小写转换
来源：http://hz.yueranfly.top/gtyshdvkxh.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.wangdashe.top/gtjansjjig.html

[R25] 去后缀 / 去前缀
来源：http://hz.cqqwz.cn/gtnagtqfmf.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.zhongyouzk.top/gtjeeyzjbt.html

[R26] 命令替换
来源：http://hz.jianghu66.top/gtqmzfinwn.html

now=$(date +%F); echo "$now"
来源：http://hz.hongshengwenyu.top/gtfoxzidpb.html

[R27] 算术展开
来源：http://hz.cucudq.cn/gtdmpzmgdr.html

echo $((1 + 2 * 3))
来源：http://hz.ppjwa.cn/gtslgfapmi.html

[R28] 浮点运算
来源：http://hz.shuidangran.top/gtbasgmyto.html

echo "scale=2; 10/3" | bc
来源：http://hz.bjfxy.top/gtsrmxbjhr.html

[R29] 定义函数
来源：http://hz.zhengqikj.top/gtszhpaact.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.hywenlv.cn/gtrbaveiyi.html

[R30] 函数返回状态码
来源：http://hz.haohaochexian.top/gtonudyzao.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.xziqi.cn/gtpkygaazq.html

[R31] 局部变量
来源：http://hz.sxryk.cn/gtaaffqanp.html

f() { local x=1; echo "$x"; }
来源：http://hz.guannengcc.top/gtntmerzqx.html

[R32] 参数个数校验
来源：http://hz.sweek.top/gtqhtbgqmn.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.dashuyun.cn/gtmzqaxufu.html

[R33] 捕获错误并提示行号
来源：http://hz.kuanghao11.cn/gtbvmkpvgv.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.zdqjudy.top/gtnccbyyfr.html

[R34] 退出时清理
来源：http://hz.jinyuanbaomall.cn/gtlkkbpogn.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.ppjwa.cn/gtkkzuwxrn.html

[R35] 后台执行并等待
来源：http://hz.guannengcc.top/gtyxyurbxi.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.jinqigfzy.top/gtvjeqgbaq.html

[R36] 并发执行多个任务
来源：http://hz.ybcxt.top/gtxmavyskp.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.zhongyouzk.top/gtfhzcngql.html

[R37] 把输出赋给变量
来源：http://hz.iojbl.cn/gtbbykqofi.html

files=$(ls -1)
来源：http://hz.gogol.net.cn/gtxpqrahlf.html

[R38] 管道串联
来源：http://hz.ppjwa.cn/gtmidlxftr.html

cat a.txt | grep -i error | wc -l
来源：http://hz.kuanghao11.cn/gtpmrqqrpn.html

[R39] 重定向标准输出与错误
来源：http://hz.ppjwa.cn/gtqhrwgpjx.html

cmd > out.log 2>&1
来源：http://hz.yj20258.top/gtqauihugw.html

[R40] 追加写日志
来源：http://hz.jinqigufen.top/gtyjpirsyt.html

echo "log" >> out.log
来源：http://hz.shanyushiyangkeji.top/gtuowdizky.html

[R41] 丢弃输出
来源：http://hz.sysykeji.top/gtmquqrhxo.html

cmd >/dev/null 2>&1
来源：http://hz.sxryk.cn/gtknmnyypk.html

[R42] 输入重定向
来源：http://hz.yvedp.cn/gtxkcuwwba.html

wc -l < a.txt
来源：http://hz.ydjk.org.cn/gtredtcsft.html

[R43] 按名字查找文件
来源：http://hz.yj202588.top/gthtcotgmy.html

find . -name "*.log" -type f
来源：http://hz.tianlin.xyz/gtpfmjvjel.html

[R44] 按修改时间查找
来源：http://hz.ywan-chungtsiang.top/gtbvfyjsmo.html

find . -mtime -7 -type f
来源：http://hz.yongpay.top/gtpxrywcfi.html

[R45] 批量删除
来源：http://hz.jqgfzy.top/gthbpmgefw.html

find . -name "*.tmp" -delete
来源：http://hz.haohaochexian.top/gtsovtztia.html

[R46] 递归替换文件内容
来源：http://hz.yuxming.cn/gtfhgfljvb.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.svipenyu.cn/gtrbkxvced.html

[R47] sed 单行替换
来源：http://hz.tian-w.cn/gtcmksybzv.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.chenjidiqi.icu/gtjyohmjop.html

[R48] awk 取指定列
来源：http://hz.jiagoushi.top/gtruaksknr.html

awk '{print $1, $3}' a.txt
来源：http://hz.jinyuanbaomall.cn/gtpoubplmt.html

[R49] awk 带条件
来源：http://hz.feifeiyinyue.top/gtrjufwafg.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.wangdashe.top/gtnteshoyi.html

[R50] awk 求和
来源：http://hz.guowangkeji.top/gtopndglyt.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.meibo888.top/gtyirwgaly.html

[R51] 排序去重取前几
来源：http://hz.sweek.top/gtdupvpmix.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.ivvv.top/gtiednbiks.html

[R52] 统计行数
来源：http://hz.cashguo.top/gtoibtlshm.html

wc -l a.txt
来源：http://hz.snrcjt.cn/gtoaqmtwpg.html

[R53] 查看文件头与实时尾
来源：http://hz.tian-w.cn/gtacpczscu.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.jyoumei.cn/gtnscguftd.html

[R54] 比较两个文件
来源：http://hz.cqqwz.cn/gtzdkzezxk.html

diff a.txt b.txt
来源：http://hz.ywan-chungtsiang.top/gtqyqoveir.html

[R55] 压缩与解压
来源：http://hz.ybcxt.top/gtqhwdapak.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.shanyushiyangtech.top/gtpjsxfdch.html

[R56] 远程拷贝
来源：http://hz.yvedp.cn/gtkdolmskl.html

scp file user@host:/path/
来源：http://hz.yanxiufei.cn/gtijtwvcex.html

[R57] 远程执行命令
来源：http://hz.jinghuilouyu.cn/gtoriezvog.html

ssh user@host 'uptime'
来源：http://hz.zdqjudy.top/gtwynkdiyz.html

[R58] 下载文件
来源：http://hz.cucudq.cn/gtlgbudkbm.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.shangyingyoupin.top/gtqkfbwawt.html

[R59] 发 POST JSON
来源：http://hz.bjfxy.top/gtdlmldupi.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.tian-w.cn/gtdzoakate.html

[R60] 只看 HTTP 状态码
来源：http://hz.cqqwz.cn/gthifbcrbv.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.gotoacloud.top/gtdnpzegpr.html

[R61] 磁盘占用
来源：http://hz.shangyingyoupin.top/gtmxwthacf.html

df -h;  du -sh *
来源：http://hz.chenlongwang.top/gtndyfhiol.html

[R62] 找最占空间的文件
来源：http://hz.tianlin.xyz/gtunfthxro.html

du -ah . | sort -rh | head -10
来源：http://hz.gotoacloud.top/gtviptnhpv.html

[R63] 内存与进程
来源：http://hz.xingfuxueyuan.xyz/gtnlrzhjfj.html

free -h;  ps aux | grep nginx
来源：http://hz.hysaishi.cn/gtnkzlthvr.html

[R64] 结束进程
来源：http://hz.sxryk.cn/gtlzseoskn.html

kill -9 $(pgrep -f app.py)
来源：http://hz.jiagoushi.top/gtibfbjfbj.html

[R65] 查看端口占用
来源：http://hz.gzhubu.top/gtgnhqzyci.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.yongpay.top/gtzvfuinmy.html

[R66] 定时任务
来源：http://hz.gaohongyu789.top/gtufwjugtt.html

crontab -e;  crontab -l
来源：http://hz.hfpthk.cn/gthunotfeg.html

[R67] 生成随机十六进制串
来源：http://hz.yangfankeji.com/gtmbetjphi.html

openssl rand -hex 16
来源：http://hz.shanyushiyangtech.top/gtbsueaamp.html

[R68] 计算文件校验值
来源：http://hz.nwbrower.top/gtqzsutqvr.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.fzhhl.top/gtunumsvxu.html

[R69] 生成随机密码
来源：http://hz.redwolf501.top/gtdxbgbxwz.html

head -c 16 /dev/urandom | base64
来源：http://hz.wangdashe.top/gtopevhozz.html

[R70] 时间戳与互转
来源：http://hz.cqqwz.cn/gtqawyzqqb.html

date +%s;  date -d @1700000000
来源：http://hz.nanxuanxn.top/gtlxkocrhi.html

[R71] 日期格式化
来源：http://hz.yuxming.cn/gthmqdmtuy.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.hywenlv.cn/gtbfhyynav.html

[R72] 等待端口就绪
来源：http://hz.gotoacloud.top/gtpbquwust.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.xziqi.cn/gtofaobpis.html

[R73] 分割大日志
来源：http://hz.redwolf501.top/gtfevknxwo.html

split -l 1000 big.log part_
来源：http://hz.xinyue.icu/gtdsbntart.html

[R74] 批量重命名
来源：http://hz.yangfankeji.com/gtwzpqjkwp.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.jinqigufen.top/gtabsaxeln.html

[R75] 导出环境变量
来源：http://hz.jiagoushi.top/gtpukdyqyg.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.shanyushiyangtech.top/gtufhfltjg.html

[R76] 使用临时文件
来源：http://hz.sufxvd.cn/gtpgalnnbq.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.jinqigfzy.top/gtpjvfnnex.html

[R77] 读取用户输入
来源：http://hz.wangdashe.top/gtoqympwlc.html

read -rp "请输入: " ans
来源：http://hz.dianchejie.cn/gttlzrrbxq.html

[R78] 交互式菜单
来源：http://hz.cdnleiting.top/gtmpmrvsmc.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.ivvv.top/gtgbxsekpw.html

[R79] 解析命令行选项
来源：http://hz.ppjwa.cn/gtxfcilbau.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.yanxiufei.cn/gtacjvthsp.html

[R80] 查看脚本执行耗时
来源：http://hz.hongshengwenyu.top/gtsviykwlh.html

time ./run.sh
来源：http://hz.c1oappe.top/gtcubakyzv.html

================================================================================
来源：http://hz.nanxinkj.top/gtingcbiwg.html

S. C / C++ 专题
来源：http://hz.hnxiangtu.top/gtzavzkgbo.html

================================================================================
来源：http://hz.hnqzz.top/gtfypazatw.html

[S01] C：Hello World
来源：http://hz.aibaodan.cn/gtivzsjvxz.html

#include <stdio.h>
来源：http://hz.zhiwuduotai.top/gtauvqaoxi.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.ydzc1.top/gtenvepzml.html

[S02] C：变量与格式化输出
来源：http://hz.daria6918.cn/gtauvffztr.html

int a = 10; printf("%d\n", a);
来源：http://hz.feifeiyinyue.top/gtntyqfand.html

[S03] C：读入整数
来源：http://hz.xziqi.cn/gtxkpvmyme.html

int x; scanf("%d", &x);
来源：http://hz.zhijiandao.cn/gttaxjdzkz.html

[S04] C：字符串复制
来源：http://hz.hammf.cn/gtzbblqzmo.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.havefunace.top/gtbfxrmhwp.html

[S05] C：字符串长度
来源：http://hz.mhx1999.top/gttweaythm.html

strlen(s)
来源：http://hz.daxiang520.top/gtechorxqp.html

[S06] C：字符串比较
来源：http://hz.xziqi.cn/gtvngkflul.html

strcmp(a, b) == 0
来源：http://hz.fengsongda.top/gtjqzjgfdx.html

[S07] C：数组遍历求和
来源：http://hz.nwbrower.top/gtpdsmpfww.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.zycfv.cn/gtnnbckjbn.html

[S08] C：动态内存分配与释放
来源：http://hz.xuetiantiany.cn/gteflnoyxh.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.shanyushiyangtech.top/gthfzekxxj.html

[S09] C：结构体定义与初始化
来源：http://hz.gaohongyu789.top/gtrajieywn.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.zhengqikj.top/gtjsgyluwv.html

[S10] C：指针与解引用
来源：http://hz.sufxvd.cn/gttpruecdu.html

int *p = &a;  *p = 5;
来源：http://hz.sysykeji.top/gtzlaiayyj.html

[S11] C：逐行读文件
来源：http://hz.svipenyu.cn/gtoxoaoebl.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.ybcxt.top/gtzypkamni.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.xziqi.cn/gtypkigrvs.html

fclose(f);
来源：http://hz.jyoumei.cn/gtcdnervsj.html

[S12] C：写文件
来源：http://hz.zhiwuduotai.top/gtihtooouh.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.ybcxt.top/gtkvaxhmhs.html

[S13] C：宏定义
来源：http://hz.zdqjudy.top/gtampqnibc.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.c1oappe.top/gtyvrwxyxt.html

[S14] C：枚举
来源：http://hz.yj202588.top/gtvievmjfd.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.zhijiandao.cn/gtmtifzibu.html

[S15] C：类型转换
来源：http://hz.yonumen.top/gtpljqbgto.html

(double) a / b
来源：http://hz.xingfuxueyuan.xyz/gtmijutkdh.html

[S16] C：位操作置位
来源：http://hz.yuxming.cn/gtjgnkrcib.html

x |= (1 << 3);
来源：http://hz.gotoacloud.top/gtahujtdim.html

[S17] C：安全拼接字符串
来源：http://hz.ybcxt.top/gtlaxuzixy.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.jiagoushi.top/gtvagekyan.html

[S18] C：命令行参数
来源：http://hz.yangfankeji.com/gtzksvmxje.html

int main(int argc, char **argv)
来源：http://hz.yuanzhike.top/gtvknobxgj.html

[S19] C：快速排序
来源：http://hz.yj20258.top/gtlexzejwj.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.ybcxt.top/gtptiqnwfz.html

[S20] C：二分查找
来源：http://hz.svipenyu.cn/gtbruerjsx.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.yueranfly.top/gtibwstakx.html

[S21] C：字符类别判断
来源：http://hz.vqdsnc.cn/gtlyhwqogx.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.jqgufenzy.top/gtyvutpaqv.html

[S22] C：字符串转数字
来源：http://hz.cheryme.top/gtkxxevrrb.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.shanyushiyangkeji.top/gtwhzyomgd.html

[S23] C：随机数
来源：http://hz.zhixingplan.top/gtvncokoxu.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.zhiwuduotai.top/gtqrkfatjw.html

[S24] C：获取本地时间
来源：http://hz.tanke756.top/gtaxnfjntb.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.zhongyouzk.top/gtddqyaotp.html

[S25] C：内存拷贝
来源：http://hz.jinqigufen.top/gtnctvxnut.html

memcpy(dst, src, n);
来源：http://hz.shangyingyoupin.top/gtyzrksmba.html

[S26] C：内存清零
来源：http://hz.shanyushiyangtech.top/gtjekutdov.html

memset(a, 0, sizeof a);
来源：http://hz.jqgfzy.top/gtuwohjprs.html

[S27] C：定义常量
来源：http://hz.fzhhl.top/gtopxnthuh.html

const double PI = 3.14159;
来源：http://hz.jyoumei.cn/gtwprfaizk.html

[S28] C：静态变量
来源：http://hz.dianchejie.cn/gtmmbioemr.html

static int counter = 0;
来源：http://hz.zhixingplan.top/gtoepnijao.html

[S29] C：变参函数
来源：http://hz.shanyushiyangtech.top/gtpprbpway.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.tanke756.top/gtwwfnsesy.html

[S30] C：头文件保护
来源：http://hz.yonumen.top/gtzjujalwc.html

#ifndef X_H
来源：http://hz.0kj1m.cn/gttaaycnqx.html

#define X_H
来源：http://hz.zhoulong.xyz/gtpiehenku.html

#endif
来源：http://hz.0kj1m.cn/gtiksszdta.html

[S31] C++：Hello World
来源：http://hz.c1oappe.top/gtftjzwxyp.html

#include <iostream>
来源：http://hz.ywan-chungtsiang.top/gtcrjyfuan.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.ydzc1.top/gtmdpdwgxp.html

[S32] C++：字符串
来源：http://hz.hysaishi.cn/gtephmdzta.html

std::string s = "hi";  s += "!";
来源：http://hz.yuanzhike.top/gtaprzfewf.html

[S33] C++：vector 增删
来源：http://hz.havefunace.top/gtsnyltvqn.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.zhiwuduotai.top/gtuyogshpg.html

[S34] C++：遍历 vector
来源：http://hz.jqgufenzy.top/gtwyylrshh.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.bjfxy.top/gthopqriqt.html

[S35] C++：map
来源：http://hz.sufxvd.cn/gtamqmpuac.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.sufxvd.cn/gtwpkgjblg.html

[S36] C++：unordered_map
来源：http://hz.guowangkeji.top/gtffvbfyli.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.52xcode.cn/gtnstvyrmd.html

[S37] C++：set
来源：http://hz.ybcxt.top/gthltgeimw.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.gaohongyu789.top/gtxmuexwus.html

[S38] C++：排序
来源：http://hz.haohaochexian.top/gtohfxtkgx.html

std::sort(v.begin(), v.end());
来源：http://hz.xuanzx.com/gtkkmpwixl.html

[S39] C++：自定义比较器排序
来源：http://hz.zhengqikj.top/gtqtsnaqdb.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.c1oappe.top/gtckklhkku.html

[S40] C++：查找元素
来源：http://hz.hammf.cn/gtyrkhzfsu.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.zhaomingkeji.xyz/gtrrzplijh.html

[S41] C++：类与构造函数
来源：http://hz.jinghuilouyu.cn/gtgilqzabm.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.dashuyun.cn/gtuqealwvr.html

[S42] C++：继承与虚函数
来源：http://hz.snrcjt.cn/gtwncboiev.html

class B : public Base { public: void f() override {} };
来源：http://hz.gzhubu.top/gtjxggrrml.html

[S43] C++：智能指针
来源：http://hz.nwbrower.top/gtrueuggsw.html

auto p = std::make_unique<int>(5);
来源：http://hz.hywenlv.cn/gtqkjgczmr.html

[S44] C++：引用传参
来源：http://hz.sxryk.cn/gtcyfnqozb.html

void inc(int &x) { ++x; }
来源：http://hz.ydzc1.top/gtlzqeorey.html

[S45] C++：lambda
来源：http://hz.jiagoushi.top/gtqlabcobf.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.tanke756.top/gtpczkssem.html

[S46] C++：函数模板
来源：http://hz.jinghuilouyu.cn/gtrtxfcsfd.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.0kj1m.cn/gtddjouktb.html


<!-- 参考信息 -->