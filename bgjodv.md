代发 wailian999

SHOW INDEX FROM users;
来源：http://hz.chenzaomai.com/gtleuemrfi.html

[Q73] 查看表状态
来源：http://hz.hysaishi.cn/gtocnzogbe.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.guannengcc.top/gtzqjajwwi.html

[Q74] 强制使用索引
来源：http://hz.xingfuxueyuan.xyz/gtqtnkxcvx.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.yanxiufei.cn/gtyiavrwdg.html

[Q75] 日期格式化
来源：http://hz.yangfankeji.com/gtjufioqmp.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.yonumen.top/gttcdtvwfo.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.pengpengdd.cyou/gtehhjsnya.html

[Q76] 按天统计
来源：http://hz.jyoumei.cn/gtjitkpihh.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.yangfankeji.com/gtkjsctacv.html

[Q77] 时间加减
来源：http://hz.jinqigufen.top/gtfcshwwui.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.zhiwuduotai.top/gtztxzjfio.html

[Q78] 当前时间
来源：http://hz.cqqwz.cn/gtkxuxgkyp.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.fengsongda.top/gtznzdzfne.html

[Q79] 字符串拼接
来源：http://hz.yuxming.cn/gtuyfhpxgg.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.yvedp.cn/gtxtawxlzj.html

[Q80] 字符串截取
来源：http://hz.fzhhl.top/gtknwlufoo.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.yj202588.top/gtbfhpgwse.html

[Q81] 字符串替换
来源：http://hz.redwolf501.top/gtpuaafqhp.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.52xcode.cn/gtdfsxmmks.html

[Q82] 字符长度与字节长度
来源：http://hz.ywan-chungtsiang.top/gthbutojex.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.0kj1m.cn/gtqlsoyocy.html

[Q83] 大小写转换
来源：http://hz.andypj.xyz/gtsqzsdyuj.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.zhixingplan.top/gtwvtdttbc.html

[Q84] 去除首尾空格
来源：http://hz.xuanzx.com/gtxhvgtblw.html

SELECT TRIM(name) FROM users;
来源：http://hz.316326.xyz/gtykrsdugr.html

[Q85] 数值取整
来源：http://hz.9152youxi.cn/gtksnuduhd.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.zycfv.cn/gtlqbqvlil.html

[Q86] 读取 JSON 字段
来源：http://hz.zhixingplan.top/gtucxulrow.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.zhongyouzk.top/gtmrgqkjxx.html

[Q87] JSON 字段做条件
来源：http://hz.ehwqpu.com/gtsvojnbej.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.hfpthk.cn/gtadvytdqe.html

[Q88] 行转列（条件聚合）
来源：http://hz.hammf.cn/gtdbilpqjs.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.nanxuanxn.top/gtthewaqbz.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.dianchejie.cn/gtcqmpxejr.html

[Q89] 判断表是否存在
来源：http://hz.yangfankeji.com/gthhjndoou.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.zhengqikj.top/gtcptbuwpd.html

[Q90] 生成序号列
来源：http://hz.iojbl.cn/gtnnhjhhls.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.ydzc1.top/gttfpqjlbh.html

================================================================================
来源：http://hz.cqqwz.cn/gtszgnupkf.html

R. Bash 专题
来源：http://hz.ivvv.top/gtirkobfew.html

================================================================================
来源：http://hz.tianlin.xyz/gtmfyfzlcf.html

[R01] shebang 与严格模式
来源：http://hz.tanke756.top/gtkenhnegw.html

#!/usr/bin/env bash
来源：http://hz.chenlongwang.top/gtnuqnvhxs.html

set -euo pipefail
来源：http://hz.aibaodan.cn/gtytmryteu.html

[R02] 变量赋值与使用
来源：http://hz.fzhhl.top/gtxeklhadi.html

name="Tom"; echo "$name"
来源：http://hz.yvedp.cn/gtiwvxykcl.html

[R03] 只读变量
来源：http://hz.jqgfzy.top/gtlkdcpsam.html

readonly PI=3.14
来源：http://hz.meibo888.top/gtapmjhzkx.html

[R04] 位置参数
来源：http://hz.52xcode.cn/gtwqqsnpma.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.mhx1999.top/gtpiykmgbk.html

[R05] 参数默认值
来源：http://hz.haohaochexian.top/gtgjfsyzfh.html

name="${1:-default}"
来源：http://hz.meibo888.top/gtfexjnoqn.html

[R06] 判断命令是否存在
来源：http://hz.shanyushiyangkeji.top/gtzkkhgvnr.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.hnqzz.top/gtggtedyyy.html

[R07] if 判断文件
来源：http://hz.hnqzz.top/gtymgefdqt.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.wangshuangyany.cn/gtcozfsrxy.html

[R08] 数值比较
来源：http://hz.redwolf501.top/gtpckfnmhw.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.jinyuanbaomall.cn/gtwmwnyezi.html

[R09] 字符串比较
来源：http://hz.jinqigufen.top/gtilmjwfnb.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.fzhhl.top/gtxiuicxol.html

[R10] 正则匹配
来源：http://hz.yongpay.top/gtgbtjsddl.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.zhaomingkeji.xyz/gtvghpieib.html

[R11] case 多分支
来源：http://hz.guowangkeji.top/gtbtnjwjus.html

case "$1" in
来源：http://hz.yj20258.top/gtdagjamrq.html

start) echo "启动" ;;
来源：http://hz.wangdashe.top/gthtvplimy.html

stop)  echo "停止" ;;
来源：http://hz.pengpengdd.cyou/gtllcxapkj.html

*)     echo "未知命令" ;;
来源：http://hz.nanxinkj.top/gtuuvogvez.html

esac
来源：http://hz.gotoacloud.top/gtypmalrdx.html

[R12] for 遍历文件
来源：http://hz.xuetiantiany.cn/gtveombhio.html

for f in *.txt; do echo "$f"; done
来源：http://hz.zhijiandao.cn/gtsqurrbis.html

[R13] for 计数循环
来源：http://hz.yuxming.cn/gttijqtrmm.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.cucudq.cn/gtbygibtqw.html

[R14] C 风格 for
来源：http://hz.fengsongda.top/gtxcvdpeal.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.jinyuanbaomall.cn/gtoienacjs.html

[R15] while 逐行读文件
来源：http://hz.hnqzz.top/gtwndoszoh.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.gaohongyu789.top/gtizyvdwsr.html

[R16] until 等待条件
来源：http://hz.aizwys.cn/gtdkhjnkvs.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.nanxuanxn.top/gtenuyvetu.html

[R17] 数组定义与取值
来源：http://hz.zhixingplan.top/gtjxcqshnj.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.ydzc1.top/gtascyewxs.html

[R18] 遍历数组
来源：http://hz.zhijiandao.cn/gtusgpeoff.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.tanke756.top/gtlwghjwrt.html

[R19] 数组长度
来源：http://hz.svipenyu.cn/gtgwlyshgo.html

echo "${#arr[@]}"
来源：http://hz.vqdsnc.cn/gtodzauycv.html

[R20] 关联数组（字典）
来源：http://hz.ehwqpu.com/gtygywyany.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.wangdashe.top/gtvkxpenky.html

[R21] 字符串长度
来源：http://hz.jianghu66.top/gtxhqxmgor.html

echo "${#s}"
来源：http://hz.shanyushiyangkeji.top/gtijlddckx.html

[R22] 截取子串
来源：http://hz.feifeiyinyue.top/gtrmlgpbud.html

echo "${s:0:5}"
来源：http://hz.iojbl.cn/gtdbhscfka.html

[R23] 字符串替换
来源：http://hz.guowangkeji.top/gthhpulhkc.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.ivvv.top/gtfcrcwyug.html

[R24] 大小写转换
来源：http://hz.cheryme.top/gtcjvsxshz.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.kuanghao11.cn/gtfwadufgr.html

[R25] 去后缀 / 去前缀
来源：http://hz.shanyushiyangtech.top/gtuaswrxgp.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.ydzc1.top/gtatmqsivm.html

[R26] 命令替换
来源：http://hz.c1oappe.top/gtcydiihzo.html

now=$(date +%F); echo "$now"
来源：http://hz.snrcjt.cn/gtitwdyoaf.html

[R27] 算术展开
来源：http://hz.cheryme.top/gtjmvvpavy.html

echo $((1 + 2 * 3))
来源：http://hz.aizwys.cn/gtzcazpmxr.html

[R28] 浮点运算
来源：http://hz.tian-w.cn/gttdagihlh.html

echo "scale=2; 10/3" | bc
来源：http://hz.shuidangran.top/gtbbmpcbzc.html

[R29] 定义函数
来源：http://hz.zhijiandao.cn/gtkokukwpd.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.guannengcc.top/gtccdjossb.html

[R30] 函数返回状态码
来源：http://hz.shzxlz.cn/gtdcuuknnl.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.bjfxy.top/gtyocyunqh.html

[R31] 局部变量
来源：http://hz.dashuyun.cn/gtxlysaoex.html

f() { local x=1; echo "$x"; }
来源：http://hz.guowangkeji.top/gtsnehtkas.html

[R32] 参数个数校验
来源：http://hz.chenzaomai.com/gtqmlyhxrs.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.svipenyu.cn/gtcwoekjec.html

[R33] 捕获错误并提示行号
来源：http://hz.tian-w.cn/gtxfqukvao.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.xingfuxueyuan.xyz/gtdkedbniz.html

[R34] 退出时清理
来源：http://hz.yueranfly.top/gtroxsngxx.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.hnqzz.top/gtalqbxrlb.html

[R35] 后台执行并等待
来源：http://hz.0kj1m.cn/gtbgwplcxb.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.xziqi.cn/gtmkabpykd.html

[R36] 并发执行多个任务
来源：http://hz.dianchejie.cn/gtldxryfal.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.yonumen.top/gtkgndvrga.html

[R37] 把输出赋给变量
来源：http://hz.xinyue.icu/gtfkmlgwgx.html

files=$(ls -1)
来源：http://hz.gotoacloud.top/gtnpmdskkd.html

[R38] 管道串联
来源：http://hz.cqqwz.cn/gtzirqysso.html

cat a.txt | grep -i error | wc -l
来源：http://hz.aibaodan.cn/gtcmcpitzp.html

[R39] 重定向标准输出与错误
来源：http://hz.dashuyun.cn/gtryumtlgh.html

cmd > out.log 2>&1
来源：http://hz.yongpay.top/gtgsiobuzv.html

[R40] 追加写日志
来源：http://hz.jianghu66.top/gtvfemgiip.html

echo "log" >> out.log
来源：http://hz.meibo888.top/gthvuvibvt.html

[R41] 丢弃输出
来源：http://hz.xingfuxueyuan.xyz/gtwnjjkdjb.html

cmd >/dev/null 2>&1
来源：http://hz.jianghu66.top/gtacevcbpi.html

[R42] 输入重定向
来源：http://hz.cheryme.top/gthwpjzopu.html

wc -l < a.txt
来源：http://hz.tian-w.cn/gtucubnbje.html

[R43] 按名字查找文件
来源：http://hz.c1oappe.top/gtnewneouc.html

find . -name "*.log" -type f
来源：http://hz.tanke756.top/gthzmlephg.html

[R44] 按修改时间查找
来源：http://hz.jiagoushi.top/gtgnjefvkk.html

find . -mtime -7 -type f
来源：http://hz.hnxiangtu.top/gtqxatxofr.html

[R45] 批量删除
来源：http://hz.zhaomingkeji.xyz/gtqchktksy.html

find . -name "*.tmp" -delete
来源：http://hz.sufxvd.cn/gtwxeznakm.html

[R46] 递归替换文件内容
来源：http://hz.xuanzx.com/gtyncxbral.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.chenlongwang.top/gtyfagavpj.html

[R47] sed 单行替换
来源：http://hz.cdnleiting.top/gtiwfawwug.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.sweek.top/gtglgfymis.html

[R48] awk 取指定列
来源：http://hz.zdqjudy.top/gtvreplurk.html

awk '{print $1, $3}' a.txt
来源：http://hz.dashuyun.cn/gtfkiraumc.html

[R49] awk 带条件
来源：http://hz.snrcjt.cn/gtsqwhcvfe.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.xinyue.icu/gtrrfbmmrf.html

[R50] awk 求和
来源：http://hz.pycfn.com/gtkycculja.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.sufxvd.cn/gtzdubcque.html

[R51] 排序去重取前几
来源：http://hz.hnxiangtu.top/gteqcvjydl.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.zhengqikj.top/gtlrshfhgo.html

[R52] 统计行数
来源：http://hz.yueranfly.top/gtqdtkprwj.html

wc -l a.txt
来源：http://hz.xuetiantiany.cn/gtklyjqydr.html

[R53] 查看文件头与实时尾
来源：http://hz.zhoulong.xyz/gtzdeyglme.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.birdmap.top/gtrfazxolp.html

[R54] 比较两个文件
来源：http://hz.gzhubu.top/gtnqppswog.html

diff a.txt b.txt
来源：http://hz.hnqzz.top/gttypvveqp.html

[R55] 压缩与解压
来源：http://hz.havefunace.top/gtzeoquhtu.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.smart0.xyz/gtkcqonlso.html

[R56] 远程拷贝
来源：http://hz.sufxvd.cn/gtinosyrid.html

scp file user@host:/path/
来源：http://hz.svipenyu.cn/gtmgirhhtb.html

[R57] 远程执行命令
来源：http://hz.zhijiandao.cn/gtaotbldwk.html

ssh user@host 'uptime'
来源：http://hz.yvedp.cn/gtlyxzcneb.html

[R58] 下载文件
来源：http://hz.c1oappe.top/gtxzhcuzyn.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.havefunace.top/gtwyrhunnf.html

[R59] 发 POST JSON
来源：http://hz.chenjidiqi.icu/gtoxxxtugp.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.mhx1999.top/gtevlqqtwm.html

[R60] 只看 HTTP 状态码
来源：http://hz.ywan-chungtsiang.top/gtpipqjaag.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.shuidangran.top/gtnwbufbds.html

[R61] 磁盘占用
来源：http://hz.9152youxi.cn/gtwajwbosp.html

df -h;  du -sh *
来源：http://hz.cucudq.cn/gtwrcoathi.html

[R62] 找最占空间的文件
来源：http://hz.redwolf501.top/gtqsrozwbr.html

du -ah . | sort -rh | head -10
来源：http://hz.guowangkeji.top/gtbmjgrrhv.html

[R63] 内存与进程
来源：http://hz.52xcode.cn/gtcefmldkf.html

free -h;  ps aux | grep nginx
来源：http://hz.hywenlv.cn/gtzadewlll.html

[R64] 结束进程
来源：http://hz.yueranfly.top/gtlgfniepg.html

kill -9 $(pgrep -f app.py)
来源：http://hz.jinqigufen.top/gtaexczlsx.html

[R65] 查看端口占用
来源：http://hz.aizwys.cn/gtzznnxpam.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.quarkkingdee.top/gtlpbicuio.html

[R66] 定时任务
来源：http://hz.daxiang520.top/gthedqgpim.html

crontab -e;  crontab -l
来源：http://hz.sysykeji.top/gtufslfrvk.html

[R67] 生成随机十六进制串
来源：http://hz.havefunace.top/gtummwpped.html

openssl rand -hex 16
来源：http://hz.fengsongda.top/gtlufswsxg.html

[R68] 计算文件校验值
来源：http://hz.chenzaomai.com/gtbntarzzf.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.jqgfzy.top/gtlxttpjrc.html

[R69] 生成随机密码
来源：http://hz.iojbl.cn/gtuubfbkbj.html

head -c 16 /dev/urandom | base64
来源：http://hz.chenzaomai.com/gtbsdkljsy.html

[R70] 时间戳与互转
来源：http://hz.chenlongwang.top/gtdihxljek.html

date +%s;  date -d @1700000000
来源：http://hz.fengsongda.top/gtbhthcxsz.html

[R71] 日期格式化
来源：http://hz.ydzc1.top/gtlkynnbva.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.cdnleiting.top/gtowklkwcx.html

[R72] 等待端口就绪
来源：http://hz.jqgfzy.top/gtqvsrjmua.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.hongshengwenyu.top/gtbbhahkcy.html

[R73] 分割大日志
来源：http://hz.feifeiyinyue.top/gtqzdtuqxx.html

split -l 1000 big.log part_
来源：http://hz.daxiang520.top/gtvuifuadb.html

[R74] 批量重命名
来源：http://hz.shuidangran.top/gtlpvixcqc.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.jlsjyb.cn/gtlkdmwvxo.html

[R75] 导出环境变量
来源：http://hz.ivvv.top/gtxmqivkja.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.hfpthk.cn/gtqeaeltwv.html

[R76] 使用临时文件
来源：http://hz.guowangkeji.top/gtdvqqvfhe.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.ivvv.top/gtdpnwlcxr.html

[R77] 读取用户输入
来源：http://hz.guowangkeji.top/gtxqcwamyb.html

read -rp "请输入: " ans
来源：http://hz.shangyingyoupin.top/gtnuwzmwun.html

[R78] 交互式菜单
来源：http://hz.sufxvd.cn/gtdugqopdp.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.jinqigufen.top/gtmtuweedt.html

[R79] 解析命令行选项
来源：http://hz.ydzc1.top/gtcdksxwim.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.yvedp.cn/gtpxxbtfkh.html

[R80] 查看脚本执行耗时
来源：http://hz.c1oappe.top/gtwdadevhc.html

time ./run.sh
来源：http://hz.bjfxy.top/gtyhnnpmif.html

================================================================================
来源：http://hz.9152youxi.cn/gtrffafuyg.html

S. C / C++ 专题
来源：http://hz.yangfankeji.com/gtmhnfoixn.html

================================================================================
来源：http://hz.svipenyu.cn/gtwciqayfn.html

[S01] C：Hello World
来源：http://hz.gotoacloud.top/gtrahglvga.html

#include <stdio.h>
来源：http://hz.yueranfly.top/gtidafzfqw.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.gogol.net.cn/gtznzyuoru.html

[S02] C：变量与格式化输出
来源：http://hz.tianlin.xyz/gtuekwcocd.html

int a = 10; printf("%d\n", a);
来源：http://hz.jianghu66.top/gtiywhqtji.html

[S03] C：读入整数
来源：http://hz.iojbl.cn/gtumneipjc.html

int x; scanf("%d", &x);
来源：http://hz.ydzc1.top/gtnqklbpcv.html

[S04] C：字符串复制
来源：http://hz.shuidangran.top/gtupcmntwh.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.ppjwa.cn/gtzcrormgz.html

[S05] C：字符串长度
来源：http://hz.chenjidiqi.icu/gttughmkuq.html

strlen(s)
来源：http://hz.jinqigfzy.top/gtijhordse.html

[S06] C：字符串比较
来源：http://hz.shzxlz.cn/gtuqlrdlur.html

strcmp(a, b) == 0
来源：http://hz.svipenyu.cn/gtpxxadobt.html

[S07] C：数组遍历求和
来源：http://hz.fzhhl.top/gtmccxhxlo.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.dianchejie.cn/gtnmncfyiy.html

[S08] C：动态内存分配与释放
来源：http://hz.jlsjyb.cn/gtprqegioj.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.hfpthk.cn/gtwyhbeepk.html

[S09] C：结构体定义与初始化
来源：http://hz.yanxiufei.cn/gtogjbknku.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.jinqigfzy.top/gtidirayzs.html

[S10] C：指针与解引用
来源：http://hz.ppjwa.cn/gtycmgjsmf.html

int *p = &a;  *p = 5;
来源：http://hz.pycfn.com/gtretuercx.html

[S11] C：逐行读文件
来源：http://hz.yueranfly.top/gtdbpnthdb.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.wangdashe.top/gtqvkdtejr.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.xingfuxueyuan.xyz/gtxbenhgig.html

fclose(f);
来源：http://hz.xinyue.icu/gtebxxjsxy.html

[S12] C：写文件
来源：http://hz.yanxiufei.cn/gtamjvgheg.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.pengpengdd.cyou/gtkjqlkxtu.html

[S13] C：宏定义
来源：http://hz.gotoacloud.top/gtllmiwrzz.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.gaohongyu789.top/gtcpnaxapc.html

[S14] C：枚举
来源：http://hz.hysaishi.cn/gtueyvosae.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.aibaodan.cn/gtxqllsrxe.html

[S15] C：类型转换
来源：http://hz.guowangkeji.top/gtjsnonkte.html

(double) a / b
来源：http://hz.quarkkingdee.top/gtjwmapzys.html

[S16] C：位操作置位
来源：http://hz.chenzaomai.com/gtwbkdvsit.html

x |= (1 << 3);
来源：http://hz.sysykeji.top/gtjbekbucz.html

[S17] C：安全拼接字符串
来源：http://hz.nanxuanxn.top/gtkrrdmrcr.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.zycfv.cn/gtbrbrplcq.html

[S18] C：命令行参数
来源：http://hz.guowangkeji.top/gtalhbbtgm.html

int main(int argc, char **argv)
来源：http://hz.wangshuangyany.cn/gtsxxzqwrb.html

[S19] C：快速排序
来源：http://hz.jlsjyb.cn/gturjepftf.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.zdqjudy.top/gtmqrjcxng.html

[S20] C：二分查找
来源：http://hz.ydjk.org.cn/gtmfjzbpcm.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.yonumen.top/gtdnbelpdc.html

[S21] C：字符类别判断
来源：http://hz.jianghu66.top/gtxislspet.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.jinqigufen.top/gtfeurpluu.html

[S22] C：字符串转数字
来源：http://hz.xingfuxueyuan.xyz/gtmnpyzfbq.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.yj20258888.top/gtztjflxcc.html

[S23] C：随机数
来源：http://hz.yangfankeji.com/gtzhynjeyq.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.pycfn.com/gtonfqoayp.html

[S24] C：获取本地时间
来源：http://hz.smart0.xyz/gtofasepmb.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.snrcjt.cn/gtqvcfnvar.html

[S25] C：内存拷贝
来源：http://hz.yj202588.top/gtphhgcjei.html

memcpy(dst, src, n);
来源：http://hz.shzxlz.cn/gttljoguuc.html

[S26] C：内存清零
来源：http://hz.yanxiufei.cn/gttmdpiakf.html

memset(a, 0, sizeof a);
来源：http://hz.dianchejie.cn/gtrwsiezbm.html

[S27] C：定义常量
来源：http://hz.ehwqpu.com/gtkjbesooc.html

const double PI = 3.14159;
来源：http://hz.9152youxi.cn/gtbdfxguvd.html

[S28] C：静态变量
来源：http://hz.yj20258.top/gtdxpwmtbe.html

static int counter = 0;
来源：http://hz.yanxiufei.cn/gtxvrygoov.html

[S29] C：变参函数
来源：http://hz.shanyushiyangtech.top/gtxppeopad.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.xylfe.cn/gtfglbluiz.html

[S30] C：头文件保护
来源：http://hz.xuetiantiany.cn/gtfabdlmyi.html

#ifndef X_H
来源：http://hz.nanxinkj.top/gtyasjadsg.html

#define X_H
来源：http://hz.c1oappe.top/gtdxntfkwx.html

#endif
来源：http://hz.jqgfzy.top/gtpqfgrupm.html

[S31] C++：Hello World
来源：http://hz.yj20258888.top/gtqbvrykba.html

#include <iostream>
来源：http://hz.smart0.xyz/gtnwatzzoo.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.sxryk.cn/gtoumlidcx.html

[S32] C++：字符串
来源：http://hz.hnqzz.top/gtxzgrgjhh.html

std::string s = "hi";  s += "!";
来源：http://hz.dashuyun.cn/gtjyagooib.html

[S33] C++：vector 增删
来源：http://hz.zhoulong.xyz/gtpfqanden.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.sysykeji.top/gtbmficwmr.html

[S34] C++：遍历 vector
来源：http://hz.jinqigfzy.top/gtjsgqzxng.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.cucudq.cn/gtaxxrfviy.html

[S35] C++：map
来源：http://hz.kuanghao11.cn/gtqdapzepf.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.gotoacloud.top/gtcdmqdenb.html

[S36] C++：unordered_map
来源：http://hz.gotoacloud.top/gtszugklsb.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.shuidangran.top/gtnbxfzvzr.html

[S37] C++：set
来源：http://hz.yj20258.top/gtkekpjzss.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.daxiang520.top/gtdxzppztb.html

[S38] C++：排序
来源：http://hz.chenlongwang.top/gtinnvttgh.html

std::sort(v.begin(), v.end());
来源：http://hz.0kj1m.cn/gtdabtbrks.html

[S39] C++：自定义比较器排序
来源：http://hz.yangfankeji.com/gtxvogpiya.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.zhijiandao.cn/gtjjbamxrg.html

[S40] C++：查找元素
来源：http://hz.0kj1m.cn/gtyuuydefn.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.yuanzhike.top/gtglvqkpri.html

[S41] C++：类与构造函数
来源：http://hz.zdqjudy.top/gtpnsvrkyn.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.guannengcc.top/gtubdpcsxy.html

[S42] C++：继承与虚函数
来源：http://hz.shuidangran.top/gtnuphgosc.html

class B : public Base { public: void f() override {} };
来源：http://hz.redwolf501.top/gtbextwwdn.html


<!-- 参考信息 -->