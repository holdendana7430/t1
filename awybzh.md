代发 wailian999

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.haohaochexian.top/gtmtoxspde.html

[Q58] 累计求和
来源：http://hz.ivvv.top/gtjcnxnilt.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.cheryme.top/gtwnagxbqk.html

[Q59] 分组内累计
来源：http://hz.yj202588.top/gtsvohshex.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.aizwys.cn/gtjquzpfim.html

[Q60] 取上一行 / 下一行
来源：http://hz.zhengqikj.top/gtcunpuihv.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.52xcode.cn/gtmiwinlvx.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.zhongyouzk.top/gtnlyxndhg.html

[Q61] 移动平均
来源：http://hz.shuidangran.top/gtieubyqgm.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.sweek.top/gtdkoirzmv.html

[Q62] 分组占比
来源：http://hz.mhx1999.top/gtjakxhsfn.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.svipenyu.cn/gtjubnuxdy.html

[Q63] 开启事务
来源：http://hz.xziqi.cn/gtaipzjlcr.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.daria6918.cn/gtpztdmnwl.html

[Q64] 提交事务
来源：http://hz.c1oappe.top/gtbpmacqrj.html

COMMIT;
来源：http://hz.nanxuanxn.top/gtjjoebljt.html

[Q65] 回滚事务
来源：http://hz.xingfuxueyuan.xyz/gtmcnxuxhc.html

ROLLBACK;
来源：http://hz.smart0.xyz/gteywtnczo.html

[Q66] 行锁查询
来源：http://hz.jyoumei.cn/gtjrdbhvhf.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.xuetiantiany.cn/gtdztuctio.html

[Q67] 设置隔离级别
来源：http://hz.sweek.top/gtowrehlfx.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.chenlongwang.top/gtcnurejfk.html

[Q68] 保存点
来源：http://hz.316326.xyz/gtvxumperu.html

SAVEPOINT sp1;
来源：http://hz.cqqwz.cn/gtpaeckwuh.html

ROLLBACK TO sp1;
来源：http://hz.quarkkingdee.top/gtksdtirry.html

[Q69] 查看执行计划
来源：http://hz.aibaodan.cn/gtasysoxxg.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.tianlin.xyz/gthiowdrks.html

[Q70] 更新统计信息
来源：http://hz.yongpay.top/gtussfcvzs.html

ANALYZE TABLE users;
来源：http://hz.nanxuanxn.top/gtopopbvyg.html

[Q71] 查看建表语句
来源：http://hz.shanyushiyangkeji.top/gttsgqbuce.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.xylfe.cn/gtpupycgip.html

[Q72] 查看索引
来源：http://hz.cdnleiting.top/gthomxzriy.html

SHOW INDEX FROM users;
来源：http://hz.zhiwuduotai.top/gtazviosjx.html

[Q73] 查看表状态
来源：http://hz.redwolf501.top/gtgkigzsue.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.jyoumei.cn/gthlweadma.html

[Q74] 强制使用索引
来源：http://hz.cdnleiting.top/gttubhaekw.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.hnqzz.top/gtcsqxwsmx.html

[Q75] 日期格式化
来源：http://hz.jqgfzy.top/gtajkoniik.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.fzhhl.top/gtfirraqyc.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.zhijiandao.cn/gtubgcgcrq.html

[Q76] 按天统计
来源：http://hz.jianghu66.top/gtaglhrush.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.smart0.xyz/gtrjuifudx.html

[Q77] 时间加减
来源：http://hz.xziqi.cn/gtpdkddvav.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.jinqigfzy.top/gtxsjhjyqd.html

[Q78] 当前时间
来源：http://hz.yj202588.top/gtxgzzulno.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.havefunace.top/gtpmpbsxpj.html

[Q79] 字符串拼接
来源：http://hz.yuanzhike.top/gtawjatzvy.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.guowangkeji.top/gtfiswiiqv.html

[Q80] 字符串截取
来源：http://hz.cqqwz.cn/gtjyvkbrrl.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.wangshuangyany.cn/gtocklqztz.html

[Q81] 字符串替换
来源：http://hz.sweek.top/gtocxrpuex.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.guowangkeji.top/gtptgfgajc.html

[Q82] 字符长度与字节长度
来源：http://hz.zhoulong.xyz/gtpiyrmefo.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.jlsjyb.cn/gtpnhginsc.html

[Q83] 大小写转换
来源：http://hz.xuetiantiany.cn/gtltmtidks.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.jianghu66.top/gtvductijm.html

[Q84] 去除首尾空格
来源：http://hz.birdmap.top/gtlhgixvfm.html

SELECT TRIM(name) FROM users;
来源：http://hz.ybcxt.top/gtcvegghhw.html

[Q85] 数值取整
来源：http://hz.feifeiyinyue.top/gtcrizfvdg.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.jinghuilouyu.cn/gtqandydtg.html

[Q86] 读取 JSON 字段
来源：http://hz.gzhubu.top/gthduiwnpi.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.yuxming.cn/gtwidjktsp.html

[Q87] JSON 字段做条件
来源：http://hz.yueranfly.top/gtsugtiljn.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.nanxinkj.top/gtcogfcrys.html

[Q88] 行转列（条件聚合）
来源：http://hz.bjfxy.top/gtumuepmys.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.sufxvd.cn/gthakfxzxs.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.jqgufenzy.top/gtouphffke.html

[Q89] 判断表是否存在
来源：http://hz.jinqigfzy.top/gtdlprsvlz.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.xuanzx.com/gtcmxmspub.html

[Q90] 生成序号列
来源：http://hz.redwolf501.top/gteaedwdby.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.yueranfly.top/gtkylgqlod.html

================================================================================
来源：http://hz.jinqigufen.top/gteryvaked.html

R. Bash 专题
来源：http://hz.aibaodan.cn/gtiqozyqpk.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtdrozedrx.html

[R01] shebang 与严格模式
来源：http://hz.yongpay.top/gtmdzpwrdj.html

#!/usr/bin/env bash
来源：http://hz.jlsjyb.cn/gtpmwjnsje.html

set -euo pipefail
来源：http://hz.ybcxt.top/gtgczjojtf.html

[R02] 变量赋值与使用
来源：http://hz.hywenlv.cn/gtkfapraag.html

name="Tom"; echo "$name"
来源：http://hz.xuanzx.com/gtykhlsnex.html

[R03] 只读变量
来源：http://hz.xuanzx.com/gtadvywxlw.html

readonly PI=3.14
来源：http://hz.aizwys.cn/gtvvugjpol.html

[R04] 位置参数
来源：http://hz.smart0.xyz/gthcinwhrd.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.havefunace.top/gtxzbuvrbt.html

[R05] 参数默认值
来源：http://hz.daria6918.cn/gtupejslls.html

name="${1:-default}"
来源：http://hz.hongshengwenyu.top/gthknpretr.html

[R06] 判断命令是否存在
来源：http://hz.zhixingplan.top/gtjugjahfy.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.cdnleiting.top/gtwazevltl.html

[R07] if 判断文件
来源：http://hz.cashguo.top/gtvovjidxb.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.jiagoushi.top/gtfezvbiwz.html

[R08] 数值比较
来源：http://hz.jianghu66.top/gtqcuyotyh.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.jqgufenzy.top/gttbkesiww.html

[R09] 字符串比较
来源：http://hz.ivvv.top/gtshnywvkv.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.316326.xyz/gtsxkafxwn.html

[R10] 正则匹配
来源：http://hz.cdnleiting.top/gtgptdboyd.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.yueranfly.top/gtnkjcasqt.html

[R11] case 多分支
来源：http://hz.cashguo.top/gtkfwpdzvb.html

case "$1" in
来源：http://hz.redwolf501.top/gtohkppgso.html

start) echo "启动" ;;
来源：http://hz.cqqwz.cn/gtdvbmcoom.html

stop)  echo "停止" ;;
来源：http://hz.aibaodan.cn/gtaxfzovce.html

*)     echo "未知命令" ;;
来源：http://hz.ivvv.top/gtynljcaki.html

esac
来源：http://hz.aizwys.cn/gtdhgqjyct.html

[R12] for 遍历文件
来源：http://hz.jiagoushi.top/gtuzbaxudl.html

for f in *.txt; do echo "$f"; done
来源：http://hz.yanxiufei.cn/gtikqjzhtl.html

[R13] for 计数循环
来源：http://hz.svipenyu.cn/gtyfxhdfkc.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.nanxuanxn.top/gtgnqjdmbe.html

[R14] C 风格 for
来源：http://hz.ivvv.top/gtelamnvzf.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.nwbrower.top/gtlkvfeoge.html

[R15] while 逐行读文件
来源：http://hz.kuanghao11.cn/gtxvcjfnus.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.guannengcc.top/gtmtwomtlo.html

[R16] until 等待条件
来源：http://hz.nwbrower.top/gtyjjdclsh.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.shuidangran.top/gtjogwxmdz.html

[R17] 数组定义与取值
来源：http://hz.haohaochexian.top/gtjetdqvnz.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.aibaodan.cn/gtawkcakip.html

[R18] 遍历数组
来源：http://hz.316326.xyz/gtompegslx.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.andypj.xyz/gtpflbmixs.html

[R19] 数组长度
来源：http://hz.aizwys.cn/gtyurtzgve.html

echo "${#arr[@]}"
来源：http://hz.yj20258888.top/gtgarkggtc.html

[R20] 关联数组（字典）
来源：http://hz.sysykeji.top/gtdlfkuifq.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.cheryme.top/gthjgrlivo.html

[R21] 字符串长度
来源：http://hz.wangshuangyany.cn/gttrdjeezb.html

echo "${#s}"
来源：http://hz.0kj1m.cn/gtlskecqiq.html

[R22] 截取子串
来源：http://hz.jinghuilouyu.cn/gtvwqiuxlh.html

echo "${s:0:5}"
来源：http://hz.feifeiyinyue.top/gttqmrycdh.html

[R23] 字符串替换
来源：http://hz.yueranfly.top/gtdbwjubls.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.zycfv.cn/gtjhfyoqyo.html

[R24] 大小写转换
来源：http://hz.guannengcc.top/gtsnguxfji.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.iojbl.cn/gtnkttbbrm.html

[R25] 去后缀 / 去前缀
来源：http://hz.yuanzhike.top/gtjdtkekrq.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.hysaishi.cn/gtalhgneah.html

[R26] 命令替换
来源：http://hz.jinghuilouyu.cn/gtxhvyntyc.html

now=$(date +%F); echo "$now"
来源：http://hz.guowangkeji.top/gtuvjaqlll.html

[R27] 算术展开
来源：http://hz.yj20258888.top/gttmkclzsi.html

echo $((1 + 2 * 3))
来源：http://hz.chenzaomai.com/gtvqxhtjva.html

[R28] 浮点运算
来源：http://hz.shanyushiyangtech.top/gtazovgbkj.html

echo "scale=2; 10/3" | bc
来源：http://hz.zhoulong.xyz/gthfycqygi.html

[R29] 定义函数
来源：http://hz.yuxming.cn/gtlayfjhff.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.daxiang520.top/gtfzltbyfx.html

[R30] 函数返回状态码
来源：http://hz.chenzaomai.com/gtvwjnfxxb.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.chenzaomai.com/gtuvgkmxuc.html

[R31] 局部变量
来源：http://hz.andypj.xyz/gtmpecyuqj.html

f() { local x=1; echo "$x"; }
来源：http://hz.cucudq.cn/gtvsicjeti.html

[R32] 参数个数校验
来源：http://hz.jinqigfzy.top/gtbjescsaz.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.xuetiantiany.cn/gttkoessxs.html

[R33] 捕获错误并提示行号
来源：http://hz.yongpay.top/gtaxaltcvg.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.bjfxy.top/gtorcaqqfo.html

[R34] 退出时清理
来源：http://hz.shuidangran.top/gtxpjevpdq.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.daria6918.cn/gtojsitmpj.html

[R35] 后台执行并等待
来源：http://hz.gogol.net.cn/gtswhwyevb.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.xuetiantiany.cn/gtdxgkgtap.html

[R36] 并发执行多个任务
来源：http://hz.cqqwz.cn/gtksbfuawt.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.hysaishi.cn/gtdeabgyeb.html

[R37] 把输出赋给变量
来源：http://hz.wangdashe.top/gtqmuosjzn.html

files=$(ls -1)
来源：http://hz.ybcxt.top/gtdmzeekiz.html

[R38] 管道串联
来源：http://hz.yangfankeji.com/gtetadzjix.html

cat a.txt | grep -i error | wc -l
来源：http://hz.yuanzhike.top/gtnalsjtzy.html

[R39] 重定向标准输出与错误
来源：http://hz.52xcode.cn/gtusdodiqw.html

cmd > out.log 2>&1
来源：http://hz.cashguo.top/gtcqbopwvl.html

[R40] 追加写日志
来源：http://hz.ydjk.org.cn/gtnalufvlw.html

echo "log" >> out.log
来源：http://hz.feifeiyinyue.top/gtpjtfovxf.html

[R41] 丢弃输出
来源：http://hz.aibaodan.cn/gtxmiwhqpt.html

cmd >/dev/null 2>&1
来源：http://hz.shuidangran.top/gtpfbmpddt.html

[R42] 输入重定向
来源：http://hz.cdnleiting.top/gtetfeytld.html

wc -l < a.txt
来源：http://hz.haohaochexian.top/gtawmyoiad.html

[R43] 按名字查找文件
来源：http://hz.smart0.xyz/gtgccmusaj.html

find . -name "*.log" -type f
来源：http://hz.316326.xyz/gtyanprnnv.html

[R44] 按修改时间查找
来源：http://hz.iojbl.cn/gtkufwcvln.html

find . -mtime -7 -type f
来源：http://hz.hysaishi.cn/gtgtzrcqmc.html

[R45] 批量删除
来源：http://hz.jinyuanbaomall.cn/gtfqedlldo.html

find . -name "*.tmp" -delete
来源：http://hz.jlsjyb.cn/gtqcpqytej.html

[R46] 递归替换文件内容
来源：http://hz.0kj1m.cn/gtixcigoec.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.c1oappe.top/gtdevwjehm.html

[R47] sed 单行替换
来源：http://hz.daxiang520.top/gtevwfryvc.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.guannengcc.top/gtmnfducsy.html

[R48] awk 取指定列
来源：http://hz.ybcxt.top/gtkyiamwde.html

awk '{print $1, $3}' a.txt
来源：http://hz.zdqjudy.top/gtxgmqocka.html

[R49] awk 带条件
来源：http://hz.tanke756.top/gtkcthnyrs.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.yj20258888.top/gtuixggxbk.html

[R50] awk 求和
来源：http://hz.nanxinkj.top/gtpsrjoydq.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.jinqigfzy.top/gtrzokapqc.html

[R51] 排序去重取前几
来源：http://hz.ydzc1.top/gtpmgxkqvi.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.zhengqikj.top/gtbjykwyrc.html

[R52] 统计行数
来源：http://hz.wangdashe.top/gttbddxpcx.html

wc -l a.txt
来源：http://hz.fzhhl.top/gtfldgdhcw.html

[R53] 查看文件头与实时尾
来源：http://hz.nwbrower.top/gtafxybton.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.xuanzx.com/gtnfrsnqfa.html

[R54] 比较两个文件
来源：http://hz.zhixingplan.top/gtcsdejenz.html

diff a.txt b.txt
来源：http://hz.zhengqikj.top/gtffnfkugu.html

[R55] 压缩与解压
来源：http://hz.jinqigfzy.top/gtbuzhmfsy.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.hywenlv.cn/gtggyqrnxn.html

[R56] 远程拷贝
来源：http://hz.daxiang520.top/gtjakjjsaq.html

scp file user@host:/path/
来源：http://hz.sysykeji.top/gtlaojvivh.html

[R57] 远程执行命令
来源：http://hz.yueranfly.top/gtcemrporx.html

ssh user@host 'uptime'
来源：http://hz.xingfuxueyuan.xyz/gtnsuvppyj.html

[R58] 下载文件
来源：http://hz.guannengcc.top/gttklpbhuj.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.sufxvd.cn/gtkncrnllr.html

[R59] 发 POST JSON
来源：http://hz.yj20258.top/gtfyybkwxv.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.xinyue.icu/gtwqgnjgzo.html

[R60] 只看 HTTP 状态码
来源：http://hz.zhengqikj.top/gtfitjzyuj.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.shangyingyoupin.top/gtmcdtxadv.html

[R61] 磁盘占用
来源：http://hz.ybcxt.top/gthpiekdtk.html

df -h;  du -sh *
来源：http://hz.xylfe.cn/gtnjrrtwwf.html

[R62] 找最占空间的文件
来源：http://hz.tian-w.cn/gtecqvlwpl.html

du -ah . | sort -rh | head -10
来源：http://hz.cucudq.cn/gthitasven.html

[R63] 内存与进程
来源：http://hz.hongshengwenyu.top/gtpipweyyx.html

free -h;  ps aux | grep nginx
来源：http://hz.yvedp.cn/gtdzeupblc.html

[R64] 结束进程
来源：http://hz.jinghuilouyu.cn/gtoqrpgwre.html

kill -9 $(pgrep -f app.py)
来源：http://hz.zhengqikj.top/gthpwnppej.html

[R65] 查看端口占用
来源：http://hz.hywenlv.cn/gttpuvmfgd.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.316326.xyz/gtznbzilay.html

[R66] 定时任务
来源：http://hz.hysaishi.cn/gtbybnmjcn.html

crontab -e;  crontab -l
来源：http://hz.316326.xyz/gtekloqvom.html

[R67] 生成随机十六进制串
来源：http://hz.hongshengwenyu.top/gtdbueiadd.html

openssl rand -hex 16
来源：http://hz.ivvv.top/gtdkmnlqdv.html

[R68] 计算文件校验值
来源：http://hz.zhijiandao.cn/gtampcsxio.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.ywan-chungtsiang.top/gtykhrlqvp.html

[R69] 生成随机密码
来源：http://hz.yuanzhike.top/gtekuhlcst.html

head -c 16 /dev/urandom | base64
来源：http://hz.ydzc1.top/gtbvynkbfe.html

[R70] 时间戳与互转
来源：http://hz.dianchejie.cn/gtjtsizein.html

date +%s;  date -d @1700000000
来源：http://hz.wangshuangyany.cn/gtzyvpasjo.html

[R71] 日期格式化
来源：http://hz.nanxinkj.top/gtdvfzdnbe.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.jinghuilouyu.cn/gtbjwdikbw.html

[R72] 等待端口就绪
来源：http://hz.9152youxi.cn/gtvwxdyrbh.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.jyoumei.cn/gtvdkzqevt.html

[R73] 分割大日志
来源：http://hz.316326.xyz/gtlumjojjm.html

split -l 1000 big.log part_
来源：http://hz.aizwys.cn/gtggpxvrlp.html

[R74] 批量重命名
来源：http://hz.nwbrower.top/gtnczupdjr.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.aizwys.cn/gtnllpluva.html

[R75] 导出环境变量
来源：http://hz.aizwys.cn/gtqbvjgqxq.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.mhx1999.top/gtljkfbpzp.html

[R76] 使用临时文件
来源：http://hz.chenzaomai.com/gtyjcutwis.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.yangfankeji.com/gtdsgcpspb.html

[R77] 读取用户输入
来源：http://hz.ppjwa.cn/gtittuivjn.html

read -rp "请输入: " ans
来源：http://hz.52xcode.cn/gtqoubrsbp.html

[R78] 交互式菜单
来源：http://hz.xinyue.icu/gtgkkiovkx.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.jianghu66.top/gtomhobhai.html

[R79] 解析命令行选项
来源：http://hz.ydjk.org.cn/gtzolvqvue.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.hammf.cn/gtmfeytfjf.html

[R80] 查看脚本执行耗时
来源：http://hz.xuetiantiany.cn/gtzoamlceb.html

time ./run.sh
来源：http://hz.hnqzz.top/gtfskqxiuy.html

================================================================================
来源：http://hz.daria6918.cn/gtorbklxju.html

S. C / C++ 专题
来源：http://hz.yuanzhike.top/gtosmrjuoa.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtybubjuct.html

[S01] C：Hello World
来源：http://hz.xylfe.cn/gtcgqyggyi.html

#include <stdio.h>
来源：http://hz.birdmap.top/gtnvqjufan.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.nanxinkj.top/gtuskopvun.html

[S02] C：变量与格式化输出
来源：http://hz.jyoumei.cn/gtblbjxmvq.html

int a = 10; printf("%d\n", a);
来源：http://hz.ydzc1.top/gtxqckhtha.html

[S03] C：读入整数
来源：http://hz.aibaodan.cn/gtepejhxiq.html

int x; scanf("%d", &x);
来源：http://hz.mhx1999.top/gttpugewml.html

[S04] C：字符串复制
来源：http://hz.zhengqikj.top/gtpzkvxofu.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.vqdsnc.cn/gtefufiauj.html

[S05] C：字符串长度
来源：http://hz.smart0.xyz/gthsfjylyi.html

strlen(s)
来源：http://hz.gaohongyu789.top/gtibleeqaf.html

[S06] C：字符串比较
来源：http://hz.chenjidiqi.icu/gttlekcwzq.html

strcmp(a, b) == 0
来源：http://hz.pycfn.com/gtsphhfwpy.html

[S07] C：数组遍历求和
来源：http://hz.hammf.cn/gtrjdvchvi.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.jinqigfzy.top/gtdmkkbuqy.html

[S08] C：动态内存分配与释放
来源：http://hz.0kj1m.cn/gtdtgardlh.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.0kj1m.cn/gtvtyjbxpl.html

[S09] C：结构体定义与初始化
来源：http://hz.nanxinkj.top/gtzcjoztvr.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.guannengcc.top/gtdezhktda.html

[S10] C：指针与解引用
来源：http://hz.cqqwz.cn/gtostqvvhs.html

int *p = &a;  *p = 5;
来源：http://hz.cheryme.top/gtwhlqgavk.html

[S11] C：逐行读文件
来源：http://hz.ivvv.top/gttadmvaai.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.yueranfly.top/gtkhljfimy.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.meibo888.top/gtqpyuclle.html

fclose(f);
来源：http://hz.sxryk.cn/gtanmdbxsg.html

[S12] C：写文件
来源：http://hz.shzxlz.cn/gtcrrxcthq.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.316326.xyz/gtmqwuvxdv.html

[S13] C：宏定义
来源：http://hz.gotoacloud.top/gtwgtdpmme.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.zdqjudy.top/gtfoxflsfb.html

[S14] C：枚举
来源：http://hz.feifeiyinyue.top/gtvimqxuvz.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.jinqigfzy.top/gtkmuwlmqn.html

[S15] C：类型转换
来源：http://hz.wangshuangyany.cn/gtexssexrg.html

(double) a / b
来源：http://hz.sweek.top/gtglvcliim.html

[S16] C：位操作置位
来源：http://hz.yj202588.top/gtjetcljwo.html

x |= (1 << 3);
来源：http://hz.yvedp.cn/gtsrvkqbyy.html

[S17] C：安全拼接字符串
来源：http://hz.birdmap.top/gtkdomkqqd.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.mhx1999.top/gtjqetjcgg.html

[S18] C：命令行参数
来源：http://hz.hywenlv.cn/gtfkmxtuzm.html

int main(int argc, char **argv)
来源：http://hz.yonumen.top/gtcfolmsei.html

[S19] C：快速排序
来源：http://hz.ivvv.top/gtwtkfwfyt.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.ivvv.top/gthnmgmofn.html

[S20] C：二分查找
来源：http://hz.iojbl.cn/gtvvpqiiqh.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.xinyue.icu/gtpbbgfrsr.html

[S21] C：字符类别判断
来源：http://hz.pengpengdd.cyou/gtznzepzmj.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.hfpthk.cn/gtvektftoa.html

[S22] C：字符串转数字
来源：http://hz.hnxiangtu.top/gtiamlnqdf.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.zhiwuduotai.top/gtfrqnznhj.html

[S23] C：随机数
来源：http://hz.pycfn.com/gtfihilbta.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.316326.xyz/gtepgxfekm.html

[S24] C：获取本地时间
来源：http://hz.yongpay.top/gtghvqbzbt.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.ivvv.top/gtgcfrdxgx.html

[S25] C：内存拷贝
来源：http://hz.zhaomingkeji.xyz/gtpxnswleu.html

memcpy(dst, src, n);
来源：http://hz.0kj1m.cn/gtowvvbueq.html

[S26] C：内存清零
来源：http://hz.shangyingyoupin.top/gtiqvupmzt.html

memset(a, 0, sizeof a);
来源：http://hz.xuanzx.com/gtxthtooiy.html

[S27] C：定义常量
来源：http://hz.zhoulong.xyz/gtrkelmenn.html

const double PI = 3.14159;
来源：http://hz.sufxvd.cn/gtcsfpumpo.html

[S28] C：静态变量
来源：http://hz.yuxming.cn/gtmkzgzkkp.html


<!-- 参考信息 -->