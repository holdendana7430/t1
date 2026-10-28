代发 wailian999

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.vqdsnc.cn/gtmklnftpi.html

[Q75] 日期格式化
来源：http://hz.yuanzhike.top/gtjpodaqui.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.gzhubu.top/gtquukhskw.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.jianghu66.top/gtcasyeliq.html

[Q76] 按天统计
来源：http://hz.jlsjyb.cn/gtrstcraje.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.tanke756.top/gtdkevxzpr.html

[Q77] 时间加减
来源：http://hz.xinyue.icu/gtjyfvxmig.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.hnxiangtu.top/gtfyzjiyem.html

[Q78] 当前时间
来源：http://hz.ehwqpu.com/gtnujghnqt.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.zhiwuduotai.top/gtfuwqimmh.html

[Q79] 字符串拼接
来源：http://hz.zhijiandao.cn/gtsnmuazzb.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.pycfn.com/gtlfikbrsb.html

[Q80] 字符串截取
来源：http://hz.jyoumei.cn/gtfyzeoozw.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.52xcode.cn/gtdiuozkan.html

[Q81] 字符串替换
来源：http://hz.hywenlv.cn/gtwbiruukv.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.gotoacloud.top/gtkwmqqwli.html

[Q82] 字符长度与字节长度
来源：http://hz.daxiang520.top/gtpnrfsuxq.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.zhongyouzk.top/gtizxeptgh.html

[Q83] 大小写转换
来源：http://hz.nanxuanxn.top/gtvztlijxr.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.guannengcc.top/gtbzknhyhk.html

[Q84] 去除首尾空格
来源：http://hz.sysykeji.top/gtkeootrdg.html

SELECT TRIM(name) FROM users;
来源：http://hz.ivvv.top/gtdgsomhws.html

[Q85] 数值取整
来源：http://hz.birdmap.top/gtdbvbdjug.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.xinyue.icu/gtflftzmff.html

[Q86] 读取 JSON 字段
来源：http://hz.xinyue.icu/gtdcdoiunz.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.yongpay.top/gtrxbfujvm.html

[Q87] JSON 字段做条件
来源：http://hz.tanke756.top/gtvntsehpc.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.bjfxy.top/gtkcylyxit.html

[Q88] 行转列（条件聚合）
来源：http://hz.vqdsnc.cn/gtpwdkbwmp.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.daxiang520.top/gtnjlunujj.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.zycfv.cn/gtjbvqsuvy.html

[Q89] 判断表是否存在
来源：http://hz.jianghu66.top/gtasethaqa.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.haohaochexian.top/gtvsapvnhv.html

[Q90] 生成序号列
来源：http://hz.ivvv.top/gtpihfodze.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.shanyushiyangkeji.top/gtnyedmviu.html

================================================================================
来源：http://hz.0kj1m.cn/gtogklfejr.html

R. Bash 专题
来源：http://hz.daria6918.cn/gtqhrvzfda.html

================================================================================
来源：http://hz.yj202588.top/gtfmkuuhfd.html

[R01] shebang 与严格模式
来源：http://hz.cashguo.top/gtjrwsieng.html

#!/usr/bin/env bash
来源：http://hz.meibo888.top/gtrjiklxnc.html

set -euo pipefail
来源：http://hz.yongpay.top/gtrdgifrjr.html

[R02] 变量赋值与使用
来源：http://hz.shuidangran.top/gtjallfdys.html

name="Tom"; echo "$name"
来源：http://hz.zhengqikj.top/gtlfsatwri.html

[R03] 只读变量
来源：http://hz.cdnleiting.top/gtijfyrdqk.html

readonly PI=3.14
来源：http://hz.zycfv.cn/gtniufcmju.html

[R04] 位置参数
来源：http://hz.zycfv.cn/gtantptyys.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.sweek.top/gtfjwflapg.html

[R05] 参数默认值
来源：http://hz.yanxiufei.cn/gthxhhyzwq.html

name="${1:-default}"
来源：http://hz.nanxuanxn.top/gtfmzdyolt.html

[R06] 判断命令是否存在
来源：http://hz.sweek.top/gtvmdrayja.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.chenzaomai.com/gtyrkyxkdh.html

[R07] if 判断文件
来源：http://hz.ywan-chungtsiang.top/gtrxznpdjc.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.iojbl.cn/gtunoxprun.html

[R08] 数值比较
来源：http://hz.zhengqikj.top/gtcyumhluw.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.xingfuxueyuan.xyz/gtrljorlgo.html

[R09] 字符串比较
来源：http://hz.cucudq.cn/gtzmrmcinm.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.zhixingplan.top/gtfyqhwlxo.html

[R10] 正则匹配
来源：http://hz.jinqigfzy.top/gteodiqujg.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.gzhubu.top/gtpqnwmtqj.html

[R11] case 多分支
来源：http://hz.jinqigufen.top/gtkviahuym.html

case "$1" in
来源：http://hz.cucudq.cn/gtczetquar.html

start) echo "启动" ;;
来源：http://hz.yuxming.cn/gtdkruujmx.html

stop)  echo "停止" ;;
来源：http://hz.ydzc1.top/gtwdajgxbd.html

*)     echo "未知命令" ;;
来源：http://hz.zhengqikj.top/gtcspoxwhl.html

esac
来源：http://hz.hongshengwenyu.top/gttgxkchbu.html

[R12] for 遍历文件
来源：http://hz.pycfn.com/gtkeuljoki.html

for f in *.txt; do echo "$f"; done
来源：http://hz.aizwys.cn/gtsduthadh.html

[R13] for 计数循环
来源：http://hz.quarkkingdee.top/gttqyhxjnd.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.yj20258.top/gtemxddaqu.html

[R14] C 风格 for
来源：http://hz.yuxming.cn/gtxmhurykd.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.aizwys.cn/gtmhxkuvaj.html

[R15] while 逐行读文件
来源：http://hz.52xcode.cn/gtyqrgyeiz.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.hfpthk.cn/gtjgmgtiwl.html

[R16] until 等待条件
来源：http://hz.ybcxt.top/gtlbmtlzfb.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.316326.xyz/gtqcnvaxpp.html

[R17] 数组定义与取值
来源：http://hz.jinqigfzy.top/gtxsaarfwd.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.nwbrower.top/gtktrtstss.html

[R18] 遍历数组
来源：http://hz.tianlin.xyz/gtekvdoyje.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.havefunace.top/gtlawnconw.html

[R19] 数组长度
来源：http://hz.xuanzx.com/gtbxwpkgse.html

echo "${#arr[@]}"
来源：http://hz.yuanzhike.top/gtstwvafou.html

[R20] 关联数组（字典）
来源：http://hz.vqdsnc.cn/gtcwhlllcb.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.hammf.cn/gtnxwhydns.html

[R21] 字符串长度
来源：http://hz.sufxvd.cn/gtwzegicec.html

echo "${#s}"
来源：http://hz.cqqwz.cn/gtwsbsjeqd.html

[R22] 截取子串
来源：http://hz.cqqwz.cn/gtpobyftqr.html

echo "${s:0:5}"
来源：http://hz.316326.xyz/gtbkwxjlvj.html

[R23] 字符串替换
来源：http://hz.yj20258.top/gtivekemhk.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.c1oappe.top/gtisfovnmm.html

[R24] 大小写转换
来源：http://hz.xuanzx.com/gtcajdhusq.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.hywenlv.cn/gtojtgvapl.html

[R25] 去后缀 / 去前缀
来源：http://hz.cashguo.top/gtizvkhvfm.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.shangyingyoupin.top/gtjhuwvuds.html

[R26] 命令替换
来源：http://hz.jqgufenzy.top/gtbhkippeo.html

now=$(date +%F); echo "$now"
来源：http://hz.52xcode.cn/gtgbwkxcwp.html

[R27] 算术展开
来源：http://hz.guannengcc.top/gtwjmoehxh.html

echo $((1 + 2 * 3))
来源：http://hz.zycfv.cn/gteaqjvxgd.html

[R28] 浮点运算
来源：http://hz.guowangkeji.top/gtfcepfglu.html

echo "scale=2; 10/3" | bc
来源：http://hz.chenlongwang.top/gthilngfhb.html

[R29] 定义函数
来源：http://hz.ydjk.org.cn/gtamtqobcx.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.0kj1m.cn/gtjcfpizuv.html

[R30] 函数返回状态码
来源：http://hz.yuanzhike.top/gtmkdofgbl.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.pycfn.com/gtphojkqhc.html

[R31] 局部变量
来源：http://hz.yanxiufei.cn/gtlpciopka.html

f() { local x=1; echo "$x"; }
来源：http://hz.pycfn.com/gtproatuhs.html

[R32] 参数个数校验
来源：http://hz.yj20258888.top/gtydoyocfo.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.nanxuanxn.top/gtofgrjpnh.html

[R33] 捕获错误并提示行号
来源：http://hz.jiagoushi.top/gthtbywfrt.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.pengpengdd.cyou/gtmgpefxos.html

[R34] 退出时清理
来源：http://hz.hnxiangtu.top/gtrcuojxqu.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.ydjk.org.cn/gtfnnbhnti.html

[R35] 后台执行并等待
来源：http://hz.sxryk.cn/gtgzynpamd.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.yonumen.top/gtxttdhvit.html

[R36] 并发执行多个任务
来源：http://hz.52xcode.cn/gtxynuquxc.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.ivvv.top/gtkndooduc.html

[R37] 把输出赋给变量
来源：http://hz.hywenlv.cn/gtdknvkfqi.html

files=$(ls -1)
来源：http://hz.jinghuilouyu.cn/gtsmxoslxf.html

[R38] 管道串联
来源：http://hz.xuetiantiany.cn/gtnsrpoelm.html

cat a.txt | grep -i error | wc -l
来源：http://hz.yuxming.cn/gtnwhqwdan.html

[R39] 重定向标准输出与错误
来源：http://hz.shangyingyoupin.top/gtledcwaoi.html

cmd > out.log 2>&1
来源：http://hz.zhaomingkeji.xyz/gtyvvvhgno.html

[R40] 追加写日志
来源：http://hz.gotoacloud.top/gtcbgfhdte.html

echo "log" >> out.log
来源：http://hz.hammf.cn/gtnpufxylb.html

[R41] 丢弃输出
来源：http://hz.ehwqpu.com/gtkkcwgohi.html

cmd >/dev/null 2>&1
来源：http://hz.sysykeji.top/gtepztqnuz.html

[R42] 输入重定向
来源：http://hz.yuanzhike.top/gtmlgbmctp.html

wc -l < a.txt
来源：http://hz.dashuyun.cn/gtlyhpowdp.html

[R43] 按名字查找文件
来源：http://hz.pycfn.com/gtaqrnvswe.html

find . -name "*.log" -type f
来源：http://hz.cqqwz.cn/gtsdikhpbd.html

[R44] 按修改时间查找
来源：http://hz.chenlongwang.top/gtonbiwjom.html

find . -mtime -7 -type f
来源：http://hz.zhongyouzk.top/gtbnstgqhc.html

[R45] 批量删除
来源：http://hz.yanxiufei.cn/gtgffaymve.html

find . -name "*.tmp" -delete
来源：http://hz.hnqzz.top/gthyqnhpte.html

[R46] 递归替换文件内容
来源：http://hz.chenlongwang.top/gtielkuxxm.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.jinqigfzy.top/gtezftegxh.html

[R47] sed 单行替换
来源：http://hz.xinyue.icu/gtolkamymr.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.fengsongda.top/gtiefkiqtn.html

[R48] awk 取指定列
来源：http://hz.jqgufenzy.top/gtzvgbrqwx.html

awk '{print $1, $3}' a.txt
来源：http://hz.ywan-chungtsiang.top/gtvkbddqmm.html

[R49] awk 带条件
来源：http://hz.sufxvd.cn/gtzhydolnw.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.zhaomingkeji.xyz/gtiwozhveb.html

[R50] awk 求和
来源：http://hz.zhengqikj.top/gtabmyxwpu.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.hywenlv.cn/gtdblsctzs.html

[R51] 排序去重取前几
来源：http://hz.snrcjt.cn/gteosjlvcz.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.cucudq.cn/gtbhjccljz.html

[R52] 统计行数
来源：http://hz.316326.xyz/gtbymjmlbp.html

wc -l a.txt
来源：http://hz.gaohongyu789.top/gtjaravozw.html

[R53] 查看文件头与实时尾
来源：http://hz.aibaodan.cn/gtwccnfuvq.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.haohaochexian.top/gtatyvjpha.html

[R54] 比较两个文件
来源：http://hz.ydzc1.top/gtiycvejtg.html

diff a.txt b.txt
来源：http://hz.pycfn.com/gtrknbulqc.html

[R55] 压缩与解压
来源：http://hz.xuanzx.com/gtfjjyygpe.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.dianchejie.cn/gtuffgxhnr.html

[R56] 远程拷贝
来源：http://hz.0kj1m.cn/gtejiooegk.html

scp file user@host:/path/
来源：http://hz.jqgufenzy.top/gtjyqvqngs.html

[R57] 远程执行命令
来源：http://hz.zhiwuduotai.top/gtgmmneccp.html

ssh user@host 'uptime'
来源：http://hz.wangshuangyany.cn/gtloadsccn.html

[R58] 下载文件
来源：http://hz.tanke756.top/gtizemvgyp.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.zhengqikj.top/gtkxrmoiqi.html

[R59] 发 POST JSON
来源：http://hz.xingfuxueyuan.xyz/gtwmwflpqf.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.nanxuanxn.top/gtvancbiyy.html

[R60] 只看 HTTP 状态码
来源：http://hz.yj20258888.top/gtlfkrhafk.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.jianghu66.top/gtkskkuloh.html

[R61] 磁盘占用
来源：http://hz.havefunace.top/gtamlloeew.html

df -h;  du -sh *
来源：http://hz.daxiang520.top/gtccyqqudb.html

[R62] 找最占空间的文件
来源：http://hz.hongshengwenyu.top/gtsqeiyfkc.html

du -ah . | sort -rh | head -10
来源：http://hz.daria6918.cn/gtkrxklrju.html

[R63] 内存与进程
来源：http://hz.yj20258888.top/gtkvykxizd.html

free -h;  ps aux | grep nginx
来源：http://hz.yj20258.top/gtsweiirry.html

[R64] 结束进程
来源：http://hz.nanxinkj.top/gtwpikwhne.html

kill -9 $(pgrep -f app.py)
来源：http://hz.smart0.xyz/gtepcaxfyk.html

[R65] 查看端口占用
来源：http://hz.cucudq.cn/gtujcreimt.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.ydzc1.top/gtjztekrby.html

[R66] 定时任务
来源：http://hz.ydjk.org.cn/gtljrmstio.html

crontab -e;  crontab -l
来源：http://hz.meibo888.top/gtqyvrpdwj.html

[R67] 生成随机十六进制串
来源：http://hz.daria6918.cn/gtfovluxyt.html

openssl rand -hex 16
来源：http://hz.zhaomingkeji.xyz/gtlpsncfqv.html

[R68] 计算文件校验值
来源：http://hz.yueranfly.top/gtudfmcnsh.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.dashuyun.cn/gtpqbeymjv.html

[R69] 生成随机密码
来源：http://hz.bjfxy.top/gtyrcklssi.html

head -c 16 /dev/urandom | base64
来源：http://hz.hnxiangtu.top/gtsunwgmin.html

[R70] 时间戳与互转
来源：http://hz.xingfuxueyuan.xyz/gttszwuebr.html

date +%s;  date -d @1700000000
来源：http://hz.jinghuilouyu.cn/gtiawoiesn.html

[R71] 日期格式化
来源：http://hz.tianlin.xyz/gtgaasmiva.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.9152youxi.cn/gtypukpiuz.html

[R72] 等待端口就绪
来源：http://hz.shangyingyoupin.top/gtnbximavj.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.ydjk.org.cn/gtyzydgcal.html

[R73] 分割大日志
来源：http://hz.redwolf501.top/gtehzvarje.html

split -l 1000 big.log part_
来源：http://hz.aibaodan.cn/gtunijdnio.html

[R74] 批量重命名
来源：http://hz.hammf.cn/gtnrbesgxr.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.zhoulong.xyz/gtkbukbkyl.html

[R75] 导出环境变量
来源：http://hz.daxiang520.top/gtwybjvcco.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.nanxuanxn.top/gtsuoeaeft.html

[R76] 使用临时文件
来源：http://hz.tian-w.cn/gtwqbbbqjh.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.zdqjudy.top/gtgnkuibqz.html

[R77] 读取用户输入
来源：http://hz.cheryme.top/gtjayrlxmy.html

read -rp "请输入: " ans
来源：http://hz.zhijiandao.cn/gteliqelec.html

[R78] 交互式菜单
来源：http://hz.jianghu66.top/gtqanktuyr.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.yuanzhike.top/gttebcovzi.html

[R79] 解析命令行选项
来源：http://hz.zhengqikj.top/gtaxdxywmb.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.havefunace.top/gtblpdmqnx.html

[R80] 查看脚本执行耗时
来源：http://hz.guowangkeji.top/gtqvcxvfqj.html

time ./run.sh
来源：http://hz.hfpthk.cn/gtkxwbxnkj.html

================================================================================
来源：http://hz.yuxming.cn/gtubtsumak.html

S. C / C++ 专题
来源：http://hz.sufxvd.cn/gtqtijmxla.html

================================================================================
来源：http://hz.gotoacloud.top/gtjibkzhjc.html

[S01] C：Hello World
来源：http://hz.iojbl.cn/gtmgftxopa.html

#include <stdio.h>
来源：http://hz.pengpengdd.cyou/gtweebdrkh.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.gogol.net.cn/gtenltfyhw.html

[S02] C：变量与格式化输出
来源：http://hz.zycfv.cn/gtcmsktulh.html

int a = 10; printf("%d\n", a);
来源：http://hz.chenzaomai.com/gtgmbqxrpl.html

[S03] C：读入整数
来源：http://hz.guannengcc.top/gteohjbksg.html

int x; scanf("%d", &x);
来源：http://hz.ybcxt.top/gtspxmfiry.html

[S04] C：字符串复制
来源：http://hz.tanke756.top/gtfamamfpu.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.hywenlv.cn/gtujvohepd.html

[S05] C：字符串长度
来源：http://hz.yj202588.top/gtudvjckex.html

strlen(s)
来源：http://hz.tianlin.xyz/gtckjunxnm.html

[S06] C：字符串比较
来源：http://hz.jiagoushi.top/gtmtjwlpix.html

strcmp(a, b) == 0
来源：http://hz.andypj.xyz/gtlpqihjou.html

[S07] C：数组遍历求和
来源：http://hz.wangshuangyany.cn/gtadurkxds.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.hongshengwenyu.top/gtjtenluit.html

[S08] C：动态内存分配与释放
来源：http://hz.zdqjudy.top/gtpitekrhq.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.kuanghao11.cn/gtscqmyrfb.html

[S09] C：结构体定义与初始化
来源：http://hz.jqgufenzy.top/gtxfgeanfl.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.tianlin.xyz/gtgyhjixrq.html

[S10] C：指针与解引用
来源：http://hz.yj20258888.top/gtgzfqeghz.html

int *p = &a;  *p = 5;
来源：http://hz.hysaishi.cn/gtuymgtsbf.html

[S11] C：逐行读文件
来源：http://hz.shuidangran.top/gtjmcvptbl.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.hongshengwenyu.top/gtsdszbnru.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.yangfankeji.com/gtgodwvrpn.html

fclose(f);
来源：http://hz.daxiang520.top/gtmzcgiizc.html

[S12] C：写文件
来源：http://hz.xuetiantiany.cn/gtepyzgcfg.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.jiagoushi.top/gtqgkvimqk.html

[S13] C：宏定义
来源：http://hz.aizwys.cn/gtjwsdaqns.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.jianghu66.top/gtbxuclnvf.html

[S14] C：枚举
来源：http://hz.svipenyu.cn/gtqvfgzdgv.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.fzhhl.top/gtjhdlerls.html

[S15] C：类型转换
来源：http://hz.jianghu66.top/gtfyploqoy.html

(double) a / b
来源：http://hz.jinghuilouyu.cn/gtfqgssewp.html

[S16] C：位操作置位
来源：http://hz.yj202588.top/gtmdpxdtgd.html

x |= (1 << 3);
来源：http://hz.cdnleiting.top/gtiurngvth.html

[S17] C：安全拼接字符串
来源：http://hz.kuanghao11.cn/gtfpdiyxbu.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.zhixingplan.top/gtxexfwtll.html

[S18] C：命令行参数
来源：http://hz.ydzc1.top/gtrzdnqyso.html

int main(int argc, char **argv)
来源：http://hz.zdqjudy.top/gtzepobydj.html

[S19] C：快速排序
来源：http://hz.cheryme.top/gtstipbnkf.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.haohaochexian.top/gtzsjpdgit.html

[S20] C：二分查找
来源：http://hz.snrcjt.cn/gtjywqzkuz.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.ydjk.org.cn/gtsgqeewsy.html

[S21] C：字符类别判断
来源：http://hz.hysaishi.cn/gtdsmcfzvs.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.zhixingplan.top/gtwaqorqzu.html

[S22] C：字符串转数字
来源：http://hz.zycfv.cn/gtavapfbfb.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.svipenyu.cn/gtrajjqdfl.html

[S23] C：随机数
来源：http://hz.cucudq.cn/gtludruxik.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.zycfv.cn/gtljxlslzk.html

[S24] C：获取本地时间
来源：http://hz.cucudq.cn/gtzvtqfxyg.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.jinghuilouyu.cn/gtbcxzvpkh.html

[S25] C：内存拷贝
来源：http://hz.tanke756.top/gtkrgqhbal.html

memcpy(dst, src, n);
来源：http://hz.gogol.net.cn/gtaptycjpb.html

[S26] C：内存清零
来源：http://hz.feifeiyinyue.top/gtotoriqjh.html

memset(a, 0, sizeof a);
来源：http://hz.bjfxy.top/gtqxoiomfb.html

[S27] C：定义常量
来源：http://hz.shuidangran.top/gtddocrrbg.html

const double PI = 3.14159;
来源：http://hz.gotoacloud.top/gtmhszxzmp.html

[S28] C：静态变量
来源：http://hz.jinghuilouyu.cn/gtgujfucny.html

static int counter = 0;
来源：http://hz.ywan-chungtsiang.top/gtpkkbabyr.html

[S29] C：变参函数
来源：http://hz.guowangkeji.top/gtbxbnajab.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.tian-w.cn/gtmypkoxrq.html

[S30] C：头文件保护
来源：http://hz.zdqjudy.top/gtbgoecssz.html

#ifndef X_H
来源：http://hz.zdqjudy.top/gtbggwezrg.html

#define X_H
来源：http://hz.yj202588.top/gtapxzjtvw.html

#endif
来源：http://hz.yongpay.top/gtxkcrfknd.html

[S31] C++：Hello World
来源：http://hz.fengsongda.top/gtktwwhpxa.html

#include <iostream>
来源：http://hz.guannengcc.top/gtihcajwhj.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.wangdashe.top/gtsctxzinl.html

[S32] C++：字符串
来源：http://hz.zycfv.cn/gtvqmnmbcb.html

std::string s = "hi";  s += "!";
来源：http://hz.yj20258.top/gtgpxqrmgp.html

[S33] C++：vector 增删
来源：http://hz.tanke756.top/gtfjhqjnfu.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.tanke756.top/gtpjcghjfh.html

[S34] C++：遍历 vector
来源：http://hz.xuetiantiany.cn/gtpsrswirv.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.dashuyun.cn/gtkourxqjq.html

[S35] C++：map
来源：http://hz.jyoumei.cn/gttbajjslw.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.fzhhl.top/gtldwsncsw.html

[S36] C++：unordered_map
来源：http://hz.sysykeji.top/gtcdifygzg.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.jinyuanbaomall.cn/gtybpzxkxi.html

[S37] C++：set
来源：http://hz.birdmap.top/gtjzlilxls.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.jinqigfzy.top/gtzyegyzlm.html

[S38] C++：排序
来源：http://hz.tanke756.top/gtpfzpjckr.html

std::sort(v.begin(), v.end());
来源：http://hz.zycfv.cn/gtpgozelma.html

[S39] C++：自定义比较器排序
来源：http://hz.xylfe.cn/gtjcatdgis.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.shzxlz.cn/gtwqkhaxyv.html

[S40] C++：查找元素
来源：http://hz.sufxvd.cn/gtytkzcbbg.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.gogol.net.cn/gtqpleeejd.html

[S41] C++：类与构造函数
来源：http://hz.xuanzx.com/gtofwqumvu.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.ywan-chungtsiang.top/gtmgssmbzl.html

[S42] C++：继承与虚函数
来源：http://hz.yuxming.cn/gtfmpwzirw.html

class B : public Base { public: void f() override {} };
来源：http://hz.jyoumei.cn/gtzrgqkuqv.html

[S43] C++：智能指针
来源：http://hz.316326.xyz/gtgosnzcqm.html

auto p = std::make_unique<int>(5);
来源：http://hz.shzxlz.cn/gtztzpndlo.html

[S44] C++：引用传参
来源：http://hz.hfpthk.cn/gtlooshokf.html

void inc(int &x) { ++x; }
来源：http://hz.nwbrower.top/gtyznfskhr.html


<!-- 参考信息 -->