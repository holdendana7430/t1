代发 wailian999

[Q67] 设置隔离级别
来源：http://hz.zhixingplan.top/gtjceapyod.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.wangshuangyany.cn/gtirmqjiaw.html

[Q68] 保存点
来源：http://hz.bjfxy.top/gtejupocny.html

SAVEPOINT sp1;
来源：http://hz.guowangkeji.top/gtvvptochg.html

ROLLBACK TO sp1;
来源：http://hz.tianlin.xyz/gtafjwcabb.html

[Q69] 查看执行计划
来源：http://hz.chenjidiqi.icu/gtdjkoaeoj.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.cucudq.cn/gtmdihydnt.html

[Q70] 更新统计信息
来源：http://hz.yj20258.top/gtiptjclta.html

ANALYZE TABLE users;
来源：http://hz.cashguo.top/gtkusxpmya.html

[Q71] 查看建表语句
来源：http://hz.hfpthk.cn/gtifszpsrt.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.daxiang520.top/gtncavhgmb.html

[Q72] 查看索引
来源：http://hz.xingfuxueyuan.xyz/gtojzueefz.html

SHOW INDEX FROM users;
来源：http://hz.xylfe.cn/gtfhdhkqre.html

[Q73] 查看表状态
来源：http://hz.gaohongyu789.top/gtsiournyj.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.pengpengdd.cyou/gtskfllhsa.html

[Q74] 强制使用索引
来源：http://hz.zhoulong.xyz/gtwszqwmju.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.jqgufenzy.top/gtiuazmphz.html

[Q75] 日期格式化
来源：http://hz.tanke756.top/gtgscfbzqt.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.chenlongwang.top/gtkcdskjts.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.hfpthk.cn/gtgxzbczht.html

[Q76] 按天统计
来源：http://hz.gaohongyu789.top/gthbshxmdo.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.snrcjt.cn/gtlczhhhio.html

[Q77] 时间加减
来源：http://hz.ybcxt.top/gtfoieoyhf.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.jqgufenzy.top/gtvevktjmo.html

[Q78] 当前时间
来源：http://hz.xylfe.cn/gtrbnyonak.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.sxryk.cn/gtaytzbjae.html

[Q79] 字符串拼接
来源：http://hz.pycfn.com/gtebpzpfuv.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.hnqzz.top/gttsrrylxq.html

[Q80] 字符串截取
来源：http://hz.hysaishi.cn/gtpsmokrno.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.shzxlz.cn/gtaifdgief.html

[Q81] 字符串替换
来源：http://hz.aizwys.cn/gtkszfuqar.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.xingfuxueyuan.xyz/gtzbgrilxo.html

[Q82] 字符长度与字节长度
来源：http://hz.hywenlv.cn/gtrrtjcojs.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.9152youxi.cn/gtlgbgniic.html

[Q83] 大小写转换
来源：http://hz.nanxinkj.top/gtiwfzctsc.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.yuanzhike.top/gtlhajnjdu.html

[Q84] 去除首尾空格
来源：http://hz.sweek.top/gtdutnqyow.html

SELECT TRIM(name) FROM users;
来源：http://hz.hfpthk.cn/gtwrvbggjb.html

[Q85] 数值取整
来源：http://hz.hnxiangtu.top/gthmubzric.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.iojbl.cn/gtxzmqomgi.html

[Q86] 读取 JSON 字段
来源：http://hz.yueranfly.top/gttisdwegq.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.xziqi.cn/gtrsaiyfhi.html

[Q87] JSON 字段做条件
来源：http://hz.52xcode.cn/gtqsrkpraa.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.chenzaomai.com/gtbawvfpxs.html

[Q88] 行转列（条件聚合）
来源：http://hz.gaohongyu789.top/gtsawuyaoh.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.aibaodan.cn/gtnsztwjaq.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.hnxiangtu.top/gtenhcshpq.html

[Q89] 判断表是否存在
来源：http://hz.chenjidiqi.icu/gtjqtmnmro.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.quarkkingdee.top/gtifldfrkh.html

[Q90] 生成序号列
来源：http://hz.yj20258888.top/gtjonblikv.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.yonumen.top/gtjdmichvb.html

================================================================================
来源：http://hz.smart0.xyz/gtgcdxdkvr.html

R. Bash 专题
来源：http://hz.hywenlv.cn/gtowrszbko.html

================================================================================
来源：http://hz.0kj1m.cn/gtvbpfucfc.html

[R01] shebang 与严格模式
来源：http://hz.quarkkingdee.top/gtzvzlrhos.html

#!/usr/bin/env bash
来源：http://hz.svipenyu.cn/gtkubvvxsd.html

set -euo pipefail
来源：http://hz.tianlin.xyz/gtfkhautjr.html

[R02] 变量赋值与使用
来源：http://hz.chenlongwang.top/gtdnteynly.html

name="Tom"; echo "$name"
来源：http://hz.cucudq.cn/gtctedfahc.html

[R03] 只读变量
来源：http://hz.zhongyouzk.top/gtpeeaenut.html

readonly PI=3.14
来源：http://hz.yonumen.top/gtffpwkudc.html

[R04] 位置参数
来源：http://hz.hnqzz.top/gtqriiaryy.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.jqgfzy.top/gtvbzwjozj.html

[R05] 参数默认值
来源：http://hz.dashuyun.cn/gtpinewzdz.html

name="${1:-default}"
来源：http://hz.yangfankeji.com/gtwbytlmlc.html

[R06] 判断命令是否存在
来源：http://hz.dashuyun.cn/gtgxnznhcn.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.9152youxi.cn/gtelwcvmge.html

[R07] if 判断文件
来源：http://hz.aizwys.cn/gtckyidoeq.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.jinqigfzy.top/gtycxbomfa.html

[R08] 数值比较
来源：http://hz.zdqjudy.top/gtbcgatesf.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.yuxming.cn/gtaosmaras.html

[R09] 字符串比较
来源：http://hz.zhijiandao.cn/gttjvwipux.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.gaohongyu789.top/gtlplfyrlh.html

[R10] 正则匹配
来源：http://hz.yueranfly.top/gtxosppdhs.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.aizwys.cn/gtyzwatzfa.html

[R11] case 多分支
来源：http://hz.zhengqikj.top/gtomcprxxe.html

case "$1" in
来源：http://hz.quarkkingdee.top/gtupuqfxli.html

start) echo "启动" ;;
来源：http://hz.vqdsnc.cn/gtjkhdiwkk.html

stop)  echo "停止" ;;
来源：http://hz.sxryk.cn/gtuhalimme.html

*)     echo "未知命令" ;;
来源：http://hz.meibo888.top/gtoztpjznc.html

esac
来源：http://hz.yanxiufei.cn/gtmrsqaqon.html

[R12] for 遍历文件
来源：http://hz.shuidangran.top/gtyzctfeze.html

for f in *.txt; do echo "$f"; done
来源：http://hz.hongshengwenyu.top/gtlhxlibct.html

[R13] for 计数循环
来源：http://hz.daria6918.cn/gttjhksqoy.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.yj20258.top/gtestvquhf.html

[R14] C 风格 for
来源：http://hz.vqdsnc.cn/gtzswtusxh.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.hongshengwenyu.top/gtqfirfzbg.html

[R15] while 逐行读文件
来源：http://hz.xingfuxueyuan.xyz/gtnqqhgcbr.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.sxryk.cn/gtrnknpbac.html

[R16] until 等待条件
来源：http://hz.zhijiandao.cn/gtgdfkrxsn.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.ydjk.org.cn/gtanwdgese.html

[R17] 数组定义与取值
来源：http://hz.gaohongyu789.top/gtozhhuztr.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.sweek.top/gtvuxeknir.html

[R18] 遍历数组
来源：http://hz.cdnleiting.top/gteauijuji.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.shanyushiyangtech.top/gtfjqnzsct.html

[R19] 数组长度
来源：http://hz.zhongyouzk.top/gtwvykscjv.html

echo "${#arr[@]}"
来源：http://hz.quarkkingdee.top/gtjyhsvbvi.html

[R20] 关联数组（字典）
来源：http://hz.jyoumei.cn/gtoqwjoiqz.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.gotoacloud.top/gtqjahddjh.html

[R21] 字符串长度
来源：http://hz.cashguo.top/gtskwoyqgd.html

echo "${#s}"
来源：http://hz.sysykeji.top/gtrocrvlts.html

[R22] 截取子串
来源：http://hz.zhiwuduotai.top/gtjyecdujq.html

echo "${s:0:5}"
来源：http://hz.jiagoushi.top/gtddugzczn.html

[R23] 字符串替换
来源：http://hz.tanke756.top/gtbzypwmxt.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.hfpthk.cn/gtclhculgb.html

[R24] 大小写转换
来源：http://hz.sxryk.cn/gtkgesnhcu.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.c1oappe.top/gtdkqzqhrg.html

[R25] 去后缀 / 去前缀
来源：http://hz.dianchejie.cn/gtjntmdakz.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.hongshengwenyu.top/gtiqhmpkcp.html

[R26] 命令替换
来源：http://hz.haohaochexian.top/gtkvkqbnha.html

now=$(date +%F); echo "$now"
来源：http://hz.xylfe.cn/gtilmvzvga.html

[R27] 算术展开
来源：http://hz.redwolf501.top/gtcatmcghu.html

echo $((1 + 2 * 3))
来源：http://hz.havefunace.top/gtrhurvznf.html

[R28] 浮点运算
来源：http://hz.shanyushiyangtech.top/gtjfefodpj.html

echo "scale=2; 10/3" | bc
来源：http://hz.zdqjudy.top/gtclafmzyu.html

[R29] 定义函数
来源：http://hz.jlsjyb.cn/gtgfymxtzq.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.iojbl.cn/gthqxhkuxi.html

[R30] 函数返回状态码
来源：http://hz.hywenlv.cn/gtnvawadra.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.ydzc1.top/gtskpqerji.html

[R31] 局部变量
来源：http://hz.daxiang520.top/gtilstalen.html

f() { local x=1; echo "$x"; }
来源：http://hz.cucudq.cn/gtcxlwzprr.html

[R32] 参数个数校验
来源：http://hz.ppjwa.cn/gtbenylnge.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.snrcjt.cn/gtumkebujq.html

[R33] 捕获错误并提示行号
来源：http://hz.birdmap.top/gtlehidjbz.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.dashuyun.cn/gtyuhhflak.html

[R34] 退出时清理
来源：http://hz.sufxvd.cn/gtkxobyuvl.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.svipenyu.cn/gteupcgmne.html

[R35] 后台执行并等待
来源：http://hz.chenzaomai.com/gtovmyzslq.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.svipenyu.cn/gtaehxureb.html

[R36] 并发执行多个任务
来源：http://hz.yuanzhike.top/gtmeizllcr.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.gogol.net.cn/gtlexhspyj.html

[R37] 把输出赋给变量
来源：http://hz.bjfxy.top/gtxjtydtbr.html

files=$(ls -1)
来源：http://hz.quarkkingdee.top/gtqflirmuj.html

[R38] 管道串联
来源：http://hz.hywenlv.cn/gtvfpvhvcs.html

cat a.txt | grep -i error | wc -l
来源：http://hz.gaohongyu789.top/gtvluvwacx.html

[R39] 重定向标准输出与错误
来源：http://hz.yangfankeji.com/gtbkgslnzd.html

cmd > out.log 2>&1
来源：http://hz.gzhubu.top/gtmczkkzqh.html

[R40] 追加写日志
来源：http://hz.daxiang520.top/gtlbatumyj.html

echo "log" >> out.log
来源：http://hz.fzhhl.top/gttjyuewqb.html

[R41] 丢弃输出
来源：http://hz.hysaishi.cn/gtqeuampky.html

cmd >/dev/null 2>&1
来源：http://hz.tanke756.top/gtawkzjsqd.html

[R42] 输入重定向
来源：http://hz.shangyingyoupin.top/gtafsjksge.html

wc -l < a.txt
来源：http://hz.redwolf501.top/gtdclszxth.html

[R43] 按名字查找文件
来源：http://hz.yj202588.top/gtlfvvhtiy.html

find . -name "*.log" -type f
来源：http://hz.ywan-chungtsiang.top/gtgvvcgnvx.html

[R44] 按修改时间查找
来源：http://hz.jinqigfzy.top/gtmsnptypt.html

find . -mtime -7 -type f
来源：http://hz.yanxiufei.cn/gtnthhdcqc.html

[R45] 批量删除
来源：http://hz.yangfankeji.com/gtzhbhhopa.html

find . -name "*.tmp" -delete
来源：http://hz.nanxuanxn.top/gtchouswyj.html

[R46] 递归替换文件内容
来源：http://hz.gzhubu.top/gtmyhoqlxd.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.ydjk.org.cn/gthjempudo.html

[R47] sed 单行替换
来源：http://hz.andypj.xyz/gthkkedhcy.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.ppjwa.cn/gtgtzycrcl.html

[R48] awk 取指定列
来源：http://hz.jinyuanbaomall.cn/gtwzvgtsql.html

awk '{print $1, $3}' a.txt
来源：http://hz.sweek.top/gtgwxbyglm.html

[R49] awk 带条件
来源：http://hz.shanyushiyangtech.top/gtfleyrujg.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.hysaishi.cn/gtdlqhxpon.html

[R50] awk 求和
来源：http://hz.gotoacloud.top/gtitqxmfia.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.dianchejie.cn/gthnagmzdk.html

[R51] 排序去重取前几
来源：http://hz.nwbrower.top/gtyduxvkjs.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.jinqigfzy.top/gtwvqkuvqv.html

[R52] 统计行数
来源：http://hz.smart0.xyz/gtsxibebkc.html

wc -l a.txt
来源：http://hz.316326.xyz/gtirkyuoqv.html

[R53] 查看文件头与实时尾
来源：http://hz.hongshengwenyu.top/gtivqyjisp.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.shuidangran.top/gtuycfvyxo.html

[R54] 比较两个文件
来源：http://hz.zhoulong.xyz/gtzeqrfolw.html

diff a.txt b.txt
来源：http://hz.chenjidiqi.icu/gtisurqjls.html

[R55] 压缩与解压
来源：http://hz.zhongyouzk.top/gtqruzmkgn.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.52xcode.cn/gtadzkipgr.html

[R56] 远程拷贝
来源：http://hz.pengpengdd.cyou/gtsrdtctqt.html

scp file user@host:/path/
来源：http://hz.daria6918.cn/gtlqyjkkdp.html

[R57] 远程执行命令
来源：http://hz.xylfe.cn/gtffzkwdbf.html

ssh user@host 'uptime'
来源：http://hz.zdqjudy.top/gtpwczyaaf.html

[R58] 下载文件
来源：http://hz.jqgufenzy.top/gtezrtsnit.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.ybcxt.top/gtyhwgxstv.html

[R59] 发 POST JSON
来源：http://hz.cashguo.top/gtjzinbnjm.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.meibo888.top/gtcqlrqnoe.html

[R60] 只看 HTTP 状态码
来源：http://hz.nanxinkj.top/gtbpceryzz.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.cucudq.cn/gtbghhxhul.html

[R61] 磁盘占用
来源：http://hz.hnxiangtu.top/gtfnxgjwoh.html

df -h;  du -sh *
来源：http://hz.cheryme.top/gthsqmlsfv.html

[R62] 找最占空间的文件
来源：http://hz.fengsongda.top/gtbajvmlfl.html

du -ah . | sort -rh | head -10
来源：http://hz.hammf.cn/gtsteuycwm.html

[R63] 内存与进程
来源：http://hz.sufxvd.cn/gtrfmgyvxz.html

free -h;  ps aux | grep nginx
来源：http://hz.haohaochexian.top/gtloipddgi.html

[R64] 结束进程
来源：http://hz.ydjk.org.cn/gtzpnnqcir.html

kill -9 $(pgrep -f app.py)
来源：http://hz.nanxuanxn.top/gtnnglpbqm.html

[R65] 查看端口占用
来源：http://hz.yj20258.top/gtkcstskgj.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.yj20258.top/gteaoitmmy.html

[R66] 定时任务
来源：http://hz.svipenyu.cn/gtpozswttb.html

crontab -e;  crontab -l
来源：http://hz.daxiang520.top/gtmjstyslg.html

[R67] 生成随机十六进制串
来源：http://hz.jinqigufen.top/gtjnznbycy.html

openssl rand -hex 16
来源：http://hz.hammf.cn/gtdfohwptr.html

[R68] 计算文件校验值
来源：http://hz.nwbrower.top/gtznevgkmc.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.snrcjt.cn/gtokfbcmxz.html

[R69] 生成随机密码
来源：http://hz.zhiwuduotai.top/gtlymsbzbs.html

head -c 16 /dev/urandom | base64
来源：http://hz.gogol.net.cn/gtuvzylxwk.html

[R70] 时间戳与互转
来源：http://hz.xuetiantiany.cn/gtuhnezhnl.html

date +%s;  date -d @1700000000
来源：http://hz.yj20258.top/gtcxfdlczx.html

[R71] 日期格式化
来源：http://hz.bjfxy.top/gtcknizsbv.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.hnxiangtu.top/gtwqwmuqon.html

[R72] 等待端口就绪
来源：http://hz.jinqigufen.top/gtogpfukgf.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.chenjidiqi.icu/gtaypwchue.html

[R73] 分割大日志
来源：http://hz.zhaomingkeji.xyz/gtsppnpnki.html

split -l 1000 big.log part_
来源：http://hz.xylfe.cn/gtklrqnnfl.html

[R74] 批量重命名
来源：http://hz.shzxlz.cn/gtdovdycxh.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.zhongyouzk.top/gtxlidqpuv.html

[R75] 导出环境变量
来源：http://hz.mhx1999.top/gtmqqrilev.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.havefunace.top/gtbzecztfv.html

[R76] 使用临时文件
来源：http://hz.chenzaomai.com/gtyvgejcmz.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.daria6918.cn/gtmxakwwcm.html

[R77] 读取用户输入
来源：http://hz.cashguo.top/gtztwfzoef.html

read -rp "请输入: " ans
来源：http://hz.yangfankeji.com/gtjaouidra.html

[R78] 交互式菜单
来源：http://hz.wangshuangyany.cn/gtmhhgawwp.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.xinyue.icu/gtzwtrvemf.html

[R79] 解析命令行选项
来源：http://hz.zycfv.cn/gtlhwpyqpx.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.jinqigfzy.top/gttpmosiru.html

[R80] 查看脚本执行耗时
来源：http://hz.jlsjyb.cn/gtirzkklam.html

time ./run.sh
来源：http://hz.yj20258888.top/gtcjzltefd.html

================================================================================
来源：http://hz.fengsongda.top/gtptckegva.html

S. C / C++ 专题
来源：http://hz.svipenyu.cn/gtgjgpwqlv.html

================================================================================
来源：http://hz.cashguo.top/gtwslfpdeb.html

[S01] C：Hello World
来源：http://hz.kuanghao11.cn/gtpydtogce.html

#include <stdio.h>
来源：http://hz.gzhubu.top/gtygiczmvi.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.zhongyouzk.top/gtztkxittf.html

[S02] C：变量与格式化输出
来源：http://hz.yonumen.top/gtixttwupy.html

int a = 10; printf("%d\n", a);
来源：http://hz.jqgfzy.top/gtpuwlsani.html

[S03] C：读入整数
来源：http://hz.meibo888.top/gtvqejyzta.html

int x; scanf("%d", &x);
来源：http://hz.fengsongda.top/gtmjksywgl.html

[S04] C：字符串复制
来源：http://hz.chenjidiqi.icu/gtmwhdqlbf.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.ppjwa.cn/gtrdfdtrnj.html

[S05] C：字符串长度
来源：http://hz.redwolf501.top/gtydjnvreq.html

strlen(s)
来源：http://hz.xingfuxueyuan.xyz/gtuhwhnqxj.html

[S06] C：字符串比较
来源：http://hz.zhiwuduotai.top/gtgdnoxfca.html

strcmp(a, b) == 0
来源：http://hz.jqgufenzy.top/gtfjhjemab.html

[S07] C：数组遍历求和
来源：http://hz.feifeiyinyue.top/gtqqnlsvpt.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.yuxming.cn/gtlcqeploc.html

[S08] C：动态内存分配与释放
来源：http://hz.xylfe.cn/gtllkubvau.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.birdmap.top/gtbcjklvyt.html

[S09] C：结构体定义与初始化
来源：http://hz.xziqi.cn/gtunexpldn.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.guowangkeji.top/gtxbayiscc.html

[S10] C：指针与解引用
来源：http://hz.ywan-chungtsiang.top/gtnivikdqf.html

int *p = &a;  *p = 5;
来源：http://hz.meibo888.top/gtihmqlcre.html

[S11] C：逐行读文件
来源：http://hz.jinyuanbaomall.cn/gtxqwsnjew.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.zhongyouzk.top/gtycqskfig.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.shzxlz.cn/gtocvtwcpq.html

fclose(f);
来源：http://hz.cqqwz.cn/gtuktaofvw.html

[S12] C：写文件
来源：http://hz.jlsjyb.cn/gthmpavjrx.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.sufxvd.cn/gtbuuuyufd.html

[S13] C：宏定义
来源：http://hz.yuanzhike.top/gteuiwecok.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.zhijiandao.cn/gtwxvtwpdd.html

[S14] C：枚举
来源：http://hz.yongpay.top/gtvmyzawbh.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.jqgfzy.top/gtwabthurt.html

[S15] C：类型转换
来源：http://hz.wangdashe.top/gtqxhnzwui.html

(double) a / b
来源：http://hz.iojbl.cn/gtogkmmrbh.html

[S16] C：位操作置位
来源：http://hz.kuanghao11.cn/gtbzeddjss.html

x |= (1 << 3);
来源：http://hz.hnxiangtu.top/gtpdojmgur.html

[S17] C：安全拼接字符串
来源：http://hz.gotoacloud.top/gtrlqnumxt.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.yanxiufei.cn/gtzyillzqc.html

[S18] C：命令行参数
来源：http://hz.xinyue.icu/gtnhtioyjl.html

int main(int argc, char **argv)
来源：http://hz.xuetiantiany.cn/gtaualnkht.html

[S19] C：快速排序
来源：http://hz.zycfv.cn/gtfhycxhvi.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.meibo888.top/gtyncofrqt.html

[S20] C：二分查找
来源：http://hz.zhiwuduotai.top/gthvgjogxc.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.jlsjyb.cn/gtmniapewn.html

[S21] C：字符类别判断
来源：http://hz.jiagoushi.top/gtjxpfbfoh.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.daria6918.cn/gtuhewwder.html

[S22] C：字符串转数字
来源：http://hz.zhijiandao.cn/gttknobyza.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.havefunace.top/gtknnonijo.html

[S23] C：随机数
来源：http://hz.sxryk.cn/gtviwjsvlk.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.andypj.xyz/gtpezcegvy.html

[S24] C：获取本地时间
来源：http://hz.0kj1m.cn/gtosxwteya.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.ywan-chungtsiang.top/gttwabklwy.html

[S25] C：内存拷贝
来源：http://hz.quarkkingdee.top/gtgivhprvl.html

memcpy(dst, src, n);
来源：http://hz.nanxinkj.top/gtwfdlouip.html

[S26] C：内存清零
来源：http://hz.ehwqpu.com/gtmteyjiju.html

memset(a, 0, sizeof a);
来源：http://hz.jinqigfzy.top/gtkrnuaylw.html

[S27] C：定义常量
来源：http://hz.hnxiangtu.top/gtzwecwsns.html

const double PI = 3.14159;
来源：http://hz.shuidangran.top/gtfnyomcqq.html

[S28] C：静态变量
来源：http://hz.guannengcc.top/gtdmedchir.html

static int counter = 0;
来源：http://hz.sysykeji.top/gtyozrhgdl.html

[S29] C：变参函数
来源：http://hz.cqqwz.cn/gtfqwiwqqv.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.haohaochexian.top/gtsjwjuygr.html

[S30] C：头文件保护
来源：http://hz.cashguo.top/gtebuqzgge.html

#ifndef X_H
来源：http://hz.aibaodan.cn/gtoimhyfxc.html

#define X_H
来源：http://hz.zhaomingkeji.xyz/gtepugebqi.html

#endif
来源：http://hz.chenzaomai.com/gtrfqilesk.html

[S31] C++：Hello World
来源：http://hz.ivvv.top/gtjtzqxezb.html

#include <iostream>
来源：http://hz.zhiwuduotai.top/gtunrfiadc.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.9152youxi.cn/gthnyaotue.html

[S32] C++：字符串
来源：http://hz.ywan-chungtsiang.top/gtpkjsooqu.html

std::string s = "hi";  s += "!";
来源：http://hz.yongpay.top/gtpewbzjxt.html

[S33] C++：vector 增删
来源：http://hz.nwbrower.top/gteuozzveh.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.yangfankeji.com/gtvwislmpr.html

[S34] C++：遍历 vector
来源：http://hz.316326.xyz/gtlyhmwxpt.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.guannengcc.top/gtimtlkcrz.html

[S35] C++：map
来源：http://hz.ywan-chungtsiang.top/gtkpcpwqcf.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.yonumen.top/gtjhefrnzl.html

[S36] C++：unordered_map
来源：http://hz.quarkkingdee.top/gtfspvodyh.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.guannengcc.top/gtwevkrgak.html


<!-- 参考信息 -->