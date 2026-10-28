代发 wailian999

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.hfpthk.cn/gtchjhknun.html

[Q56] 密集排名（并列不占位）
来源：http://hz.dianchejie.cn/gtkpbwxuav.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.redwolf501.top/gtximrwmnz.html

[Q57] 行号
来源：http://hz.jqgfzy.top/gtupxukgkj.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.cdnleiting.top/gtepuwdyto.html

[Q58] 累计求和
来源：http://hz.yvedp.cn/gtdwnfbasj.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.nanxuanxn.top/gthwfwqkdt.html

[Q59] 分组内累计
来源：http://hz.nanxinkj.top/gttwqneoil.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.nwbrower.top/gtpdfbhfzk.html

[Q60] 取上一行 / 下一行
来源：http://hz.guannengcc.top/gtnxvzlcay.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.wangshuangyany.cn/gtyavgtrqs.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.cheryme.top/gtaavflgex.html

[Q61] 移动平均
来源：http://hz.xziqi.cn/gtaczviyoo.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.0kj1m.cn/gtefredvpk.html

[Q62] 分组占比
来源：http://hz.aizwys.cn/gtooyyecwk.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.yj202588.top/gtybavabcc.html

[Q63] 开启事务
来源：http://hz.chenlongwang.top/gtcigkgjfc.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.ydjk.org.cn/gtmwvjmdvf.html

[Q64] 提交事务
来源：http://hz.kuanghao11.cn/gtjhaeyqno.html

COMMIT;
来源：http://hz.shangyingyoupin.top/gtssxuxioj.html

[Q65] 回滚事务
来源：http://hz.tian-w.cn/gtnfgdwwsz.html

ROLLBACK;
来源：http://hz.zhixingplan.top/gtrhdiqzti.html

[Q66] 行锁查询
来源：http://hz.cheryme.top/gtyxeqzevk.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.gzhubu.top/gtoujehbcc.html

[Q67] 设置隔离级别
来源：http://hz.jiagoushi.top/gtpjjfmbuj.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.ydjk.org.cn/gtbdzxixdw.html

[Q68] 保存点
来源：http://hz.jiagoushi.top/gtfdrwtjlw.html

SAVEPOINT sp1;
来源：http://hz.ydzc1.top/gthzkxsvqr.html

ROLLBACK TO sp1;
来源：http://hz.fengsongda.top/gteczyebjp.html

[Q69] 查看执行计划
来源：http://hz.zdqjudy.top/gtysiylmom.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.9152youxi.cn/gtocfeuogg.html

[Q70] 更新统计信息
来源：http://hz.pengpengdd.cyou/gtknzvinsh.html

ANALYZE TABLE users;
来源：http://hz.snrcjt.cn/gthfomjqid.html

[Q71] 查看建表语句
来源：http://hz.snrcjt.cn/gtktkstbtp.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.chenzaomai.com/gtystxneal.html

[Q72] 查看索引
来源：http://hz.wangshuangyany.cn/gtbpzxylzb.html

SHOW INDEX FROM users;
来源：http://hz.ppjwa.cn/gtkhaqkkck.html

[Q73] 查看表状态
来源：http://hz.hongshengwenyu.top/gtqsmsecbs.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.ehwqpu.com/gtytacqjbr.html

[Q74] 强制使用索引
来源：http://hz.jqgufenzy.top/gtsoylvxcm.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.zhongyouzk.top/gtixysxrxy.html

[Q75] 日期格式化
来源：http://hz.yuanzhike.top/gtrfxazeyj.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.guannengcc.top/gtkosjdugt.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.cheryme.top/gtbnpicuvi.html

[Q76] 按天统计
来源：http://hz.hnqzz.top/gtdgqsridq.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.cqqwz.cn/gtaoipfqij.html

[Q77] 时间加减
来源：http://hz.ivvv.top/gtmciyudrd.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.hysaishi.cn/gtnwszhipc.html

[Q78] 当前时间
来源：http://hz.jinyuanbaomall.cn/gtldaadiui.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.tanke756.top/gtjabgxvan.html

[Q79] 字符串拼接
来源：http://hz.gaohongyu789.top/gtfmrxblfh.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.nwbrower.top/gthxpxnoqd.html

[Q80] 字符串截取
来源：http://hz.smart0.xyz/gtdloissoc.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.fzhhl.top/gtgqqfwlwe.html

[Q81] 字符串替换
来源：http://hz.jlsjyb.cn/gtlfkzosat.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.hfpthk.cn/gtpxkmvjuv.html

[Q82] 字符长度与字节长度
来源：http://hz.cqqwz.cn/gtxrhslrro.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.tian-w.cn/gtwmsmiprz.html

[Q83] 大小写转换
来源：http://hz.yuanzhike.top/gtoxvrmvpo.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.xuetiantiany.cn/gtnodzamgt.html

[Q84] 去除首尾空格
来源：http://hz.ydjk.org.cn/gtdsaymtuc.html

SELECT TRIM(name) FROM users;
来源：http://hz.fengsongda.top/gtgruvncsd.html

[Q85] 数值取整
来源：http://hz.bjfxy.top/gtoeesqkhs.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.xziqi.cn/gttsehyfwv.html

[Q86] 读取 JSON 字段
来源：http://hz.jqgfzy.top/gtmszemoia.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.zhijiandao.cn/gtmohoshrt.html

[Q87] JSON 字段做条件
来源：http://hz.zhaomingkeji.xyz/gtrkgskffh.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.nanxinkj.top/gtjmzfuvfa.html

[Q88] 行转列（条件聚合）
来源：http://hz.chenzaomai.com/gtjhopbwba.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.pengpengdd.cyou/gttkxodjwc.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.zycfv.cn/gtaooyloiz.html

[Q89] 判断表是否存在
来源：http://hz.jinghuilouyu.cn/gtlarkklas.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.feifeiyinyue.top/gtohmcalaw.html

[Q90] 生成序号列
来源：http://hz.xylfe.cn/gtoutcobej.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.shanyushiyangkeji.top/gtoirdtspz.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtfvmkjgpo.html

R. Bash 专题
来源：http://hz.yj20258888.top/gtisvyycnt.html

================================================================================
来源：http://hz.ydzc1.top/gtqkbqzscq.html

[R01] shebang 与严格模式
来源：http://hz.dashuyun.cn/gtswzjkcen.html

#!/usr/bin/env bash
来源：http://hz.shuidangran.top/gtprnncabb.html

set -euo pipefail
来源：http://hz.guannengcc.top/gtxbhgadqa.html

[R02] 变量赋值与使用
来源：http://hz.wangshuangyany.cn/gtknmwsgjt.html

name="Tom"; echo "$name"
来源：http://hz.zdqjudy.top/gtunychbcf.html

[R03] 只读变量
来源：http://hz.jqgfzy.top/gtukrpnxey.html

readonly PI=3.14
来源：http://hz.chenjidiqi.icu/gtsrxtvjzl.html

[R04] 位置参数
来源：http://hz.zhaomingkeji.xyz/gtyjllasjm.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.tanke756.top/gtcmuxszqk.html

[R05] 参数默认值
来源：http://hz.birdmap.top/gthfywkjnt.html

name="${1:-default}"
来源：http://hz.shzxlz.cn/gtahpccmqx.html

[R06] 判断命令是否存在
来源：http://hz.jinqigfzy.top/gtzfkgtrqi.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.dianchejie.cn/gttbbtpfsy.html

[R07] if 判断文件
来源：http://hz.redwolf501.top/gtzluklnyw.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.gotoacloud.top/gtiqvfawlp.html

[R08] 数值比较
来源：http://hz.jianghu66.top/gtyujjsmkz.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.9152youxi.cn/gtkqhuljzl.html

[R09] 字符串比较
来源：http://hz.cashguo.top/gtevowbibl.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.jinyuanbaomall.cn/gtxjdgkszk.html

[R10] 正则匹配
来源：http://hz.jianghu66.top/gtbllqcfuo.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.hysaishi.cn/gthliepvtx.html

[R11] case 多分支
来源：http://hz.ydjk.org.cn/gtidiutfqj.html

case "$1" in
来源：http://hz.svipenyu.cn/gtjuwyagzc.html

start) echo "启动" ;;
来源：http://hz.zdqjudy.top/gtzzrpottx.html

stop)  echo "停止" ;;
来源：http://hz.gotoacloud.top/gtqolccqhb.html

*)     echo "未知命令" ;;
来源：http://hz.52xcode.cn/gtmftwqfpa.html

esac
来源：http://hz.andypj.xyz/gtsxjvxhyd.html

[R12] for 遍历文件
来源：http://hz.meibo888.top/gtaurudxys.html

for f in *.txt; do echo "$f"; done
来源：http://hz.chenlongwang.top/gtasovbqns.html

[R13] for 计数循环
来源：http://hz.ydzc1.top/gttcpxlgva.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.sxryk.cn/gtkcjatysl.html

[R14] C 风格 for
来源：http://hz.ehwqpu.com/gtcvyjvdrn.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.dianchejie.cn/gtzqxxeife.html

[R15] while 逐行读文件
来源：http://hz.pycfn.com/gtsaxllrjs.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.shuidangran.top/gtcethlckd.html

[R16] until 等待条件
来源：http://hz.iojbl.cn/gtnkvbgcdp.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.zhoulong.xyz/gtiohjrede.html

[R17] 数组定义与取值
来源：http://hz.dianchejie.cn/gtcdkhfxvm.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.snrcjt.cn/gtydfwyztv.html

[R18] 遍历数组
来源：http://hz.ydzc1.top/gtxvlhgtgd.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.aizwys.cn/gtmhmhqsyq.html

[R19] 数组长度
来源：http://hz.dashuyun.cn/gtbskzrqnt.html

echo "${#arr[@]}"
来源：http://hz.zhiwuduotai.top/gtobtmsxah.html

[R20] 关联数组（字典）
来源：http://hz.daxiang520.top/gtmjwwvcnl.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.nanxinkj.top/gtdkxogjgn.html

[R21] 字符串长度
来源：http://hz.birdmap.top/gtunxszshf.html

echo "${#s}"
来源：http://hz.xziqi.cn/gttcvmauzd.html

[R22] 截取子串
来源：http://hz.mhx1999.top/gtjssdiqjw.html

echo "${s:0:5}"
来源：http://hz.xuanzx.com/gtnmppewjj.html

[R23] 字符串替换
来源：http://hz.ywan-chungtsiang.top/gtarvgpmft.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.meibo888.top/gtrblienbq.html

[R24] 大小写转换
来源：http://hz.sxryk.cn/gtwkwjieij.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.ppjwa.cn/gtxczuvbhf.html

[R25] 去后缀 / 去前缀
来源：http://hz.zhaomingkeji.xyz/gtvustzzle.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.wangshuangyany.cn/gtyfjhikuy.html

[R26] 命令替换
来源：http://hz.jianghu66.top/gtshrmdihx.html

now=$(date +%F); echo "$now"
来源：http://hz.nanxinkj.top/gtxuzequsv.html

[R27] 算术展开
来源：http://hz.nanxuanxn.top/gtaotanupn.html

echo $((1 + 2 * 3))
来源：http://hz.yonumen.top/gtaarfnhbe.html

[R28] 浮点运算
来源：http://hz.havefunace.top/gtdocimkwz.html

echo "scale=2; 10/3" | bc
来源：http://hz.quarkkingdee.top/gtsfiujavz.html

[R29] 定义函数
来源：http://hz.aizwys.cn/gtxyedaqpu.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.zhengqikj.top/gtavfyzvrt.html

[R30] 函数返回状态码
来源：http://hz.cheryme.top/gtcexqpeod.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.hfpthk.cn/gteskenxfl.html

[R31] 局部变量
来源：http://hz.pycfn.com/gtqleiswki.html

f() { local x=1; echo "$x"; }
来源：http://hz.yonumen.top/gtopgjwmcv.html

[R32] 参数个数校验
来源：http://hz.zhixingplan.top/gtcbhsqfxz.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.zhijiandao.cn/gtubcagkph.html

[R33] 捕获错误并提示行号
来源：http://hz.yuxming.cn/gtmbkpdrsl.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.sxryk.cn/gtznzmkxpq.html

[R34] 退出时清理
来源：http://hz.zycfv.cn/gtjlzqlygt.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.nanxinkj.top/gtbtbsaljt.html

[R35] 后台执行并等待
来源：http://hz.xuetiantiany.cn/gthjepahbu.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.meibo888.top/gtysvxdghc.html

[R36] 并发执行多个任务
来源：http://hz.jlsjyb.cn/gtrlvlzici.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.zhiwuduotai.top/gtlnjtusux.html

[R37] 把输出赋给变量
来源：http://hz.cheryme.top/gtaknpmgez.html

files=$(ls -1)
来源：http://hz.c1oappe.top/gtazkfqnis.html

[R38] 管道串联
来源：http://hz.ydzc1.top/gtgebpdmni.html

cat a.txt | grep -i error | wc -l
来源：http://hz.ivvv.top/gtjlxujjyl.html

[R39] 重定向标准输出与错误
来源：http://hz.ybcxt.top/gthewluppt.html

cmd > out.log 2>&1
来源：http://hz.yanxiufei.cn/gtdgmumstu.html

[R40] 追加写日志
来源：http://hz.sysykeji.top/gtbfisowmx.html

echo "log" >> out.log
来源：http://hz.pycfn.com/gticaornjg.html

[R41] 丢弃输出
来源：http://hz.shzxlz.cn/gtcjdtntuk.html

cmd >/dev/null 2>&1
来源：http://hz.sysykeji.top/gtwwrsibkb.html

[R42] 输入重定向
来源：http://hz.hnqzz.top/gtrvgqpfvh.html

wc -l < a.txt
来源：http://hz.vqdsnc.cn/gtjqnaydod.html

[R43] 按名字查找文件
来源：http://hz.cashguo.top/gtlfvcudja.html

find . -name "*.log" -type f
来源：http://hz.ydjk.org.cn/gtbqebudde.html

[R44] 按修改时间查找
来源：http://hz.shangyingyoupin.top/gtfbqfrhsc.html

find . -mtime -7 -type f
来源：http://hz.nanxinkj.top/gtsjaklnfm.html

[R45] 批量删除
来源：http://hz.aibaodan.cn/gtnwxtloxd.html

find . -name "*.tmp" -delete
来源：http://hz.nanxuanxn.top/gtswqukdzl.html

[R46] 递归替换文件内容
来源：http://hz.yonumen.top/gtsduvnuzl.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.andypj.xyz/gtwpndbgxb.html

[R47] sed 单行替换
来源：http://hz.fzhhl.top/gtjwypmhok.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.shanyushiyangtech.top/gtudywhcoy.html

[R48] awk 取指定列
来源：http://hz.pengpengdd.cyou/gtaqmamlcb.html

awk '{print $1, $3}' a.txt
来源：http://hz.feifeiyinyue.top/gtsayjpmmh.html

[R49] awk 带条件
来源：http://hz.zhengqikj.top/gthieywoin.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.jyoumei.cn/gtwxnfhwts.html

[R50] awk 求和
来源：http://hz.0kj1m.cn/gtpnytkseo.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.yangfankeji.com/gtdxezjijf.html

[R51] 排序去重取前几
来源：http://hz.tanke756.top/gtextttchp.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.gzhubu.top/gtvrzbfcxn.html

[R52] 统计行数
来源：http://hz.chenlongwang.top/gtgouutwxx.html

wc -l a.txt
来源：http://hz.gotoacloud.top/gteazlubyb.html

[R53] 查看文件头与实时尾
来源：http://hz.ivvv.top/gtfwccmvpk.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.xinyue.icu/gtcgnizmef.html

[R54] 比较两个文件
来源：http://hz.nanxuanxn.top/gtzoxvtzjx.html

diff a.txt b.txt
来源：http://hz.jqgfzy.top/gthivlzflz.html

[R55] 压缩与解压
来源：http://hz.jlsjyb.cn/gtndfdjavq.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.zhongyouzk.top/gtryznpwcv.html

[R56] 远程拷贝
来源：http://hz.jinqigfzy.top/gtqdjvjmcz.html

scp file user@host:/path/
来源：http://hz.chenzaomai.com/gtyqonffpl.html

[R57] 远程执行命令
来源：http://hz.xuanzx.com/gtyppjdywa.html

ssh user@host 'uptime'
来源：http://hz.wangdashe.top/gtzyirvnkk.html

[R58] 下载文件
来源：http://hz.tian-w.cn/gtvtugzfni.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.shanyushiyangkeji.top/gtncnlqxux.html

[R59] 发 POST JSON
来源：http://hz.shangyingyoupin.top/gtqggamvsy.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.hammf.cn/gtaucwenlh.html

[R60] 只看 HTTP 状态码
来源：http://hz.zhiwuduotai.top/gtuukghukq.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.birdmap.top/gtfevrvgyo.html

[R61] 磁盘占用
来源：http://hz.iojbl.cn/gtvigrnfbc.html

df -h;  du -sh *
来源：http://hz.zhoulong.xyz/gtmhmceney.html

[R62] 找最占空间的文件
来源：http://hz.bjfxy.top/gteyrtuxxg.html

du -ah . | sort -rh | head -10
来源：http://hz.52xcode.cn/gtqqmuytbj.html

[R63] 内存与进程
来源：http://hz.wangdashe.top/gtntlbhkxc.html

free -h;  ps aux | grep nginx
来源：http://hz.jinghuilouyu.cn/gtdiiayeej.html

[R64] 结束进程
来源：http://hz.tianlin.xyz/gtuhxfatpw.html

kill -9 $(pgrep -f app.py)
来源：http://hz.zhiwuduotai.top/gtgpawvtle.html

[R65] 查看端口占用
来源：http://hz.zhiwuduotai.top/gttfvhuefh.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.svipenyu.cn/gtyeezmshp.html

[R66] 定时任务
来源：http://hz.zhixingplan.top/gtpfdxotaf.html

crontab -e;  crontab -l
来源：http://hz.cqqwz.cn/gthwsqxuyf.html

[R67] 生成随机十六进制串
来源：http://hz.gzhubu.top/gtbixnhnix.html

openssl rand -hex 16
来源：http://hz.sufxvd.cn/gteqiqpycr.html

[R68] 计算文件校验值
来源：http://hz.guannengcc.top/gtjbuipprr.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.zycfv.cn/gtefwefttz.html

[R69] 生成随机密码
来源：http://hz.zhaomingkeji.xyz/gtwtdedqzv.html

head -c 16 /dev/urandom | base64
来源：http://hz.zhixingplan.top/gtnuvdddmr.html

[R70] 时间戳与互转
来源：http://hz.pengpengdd.cyou/gtlameuvhq.html

date +%s;  date -d @1700000000
来源：http://hz.cucudq.cn/gttgbqszij.html

[R71] 日期格式化
来源：http://hz.zdqjudy.top/gtrlbhqnim.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.dianchejie.cn/gtqiusitvh.html

[R72] 等待端口就绪
来源：http://hz.yongpay.top/gttowwuzpz.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.ywan-chungtsiang.top/gtkqjpeivh.html

[R73] 分割大日志
来源：http://hz.daxiang520.top/gtyrjflmxb.html

split -l 1000 big.log part_
来源：http://hz.zhixingplan.top/gtnqyqjgmz.html

[R74] 批量重命名
来源：http://hz.hongshengwenyu.top/gtoxkdayof.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.cheryme.top/gtbjmrnxce.html

[R75] 导出环境变量
来源：http://hz.wangdashe.top/gtgxvmekik.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.redwolf501.top/gtgqsxbhlf.html

[R76] 使用临时文件
来源：http://hz.yj202588.top/gtqzmomeea.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.iojbl.cn/gtawsytfwq.html

[R77] 读取用户输入
来源：http://hz.chenjidiqi.icu/gtdzlqndfs.html

read -rp "请输入: " ans
来源：http://hz.jqgufenzy.top/gtynlipbhk.html

[R78] 交互式菜单
来源：http://hz.yj20258888.top/gttcmxcnnq.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.birdmap.top/gttdsjthre.html

[R79] 解析命令行选项
来源：http://hz.jinqigfzy.top/gthzjvqilt.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.nwbrower.top/gteheaxywh.html

[R80] 查看脚本执行耗时
来源：http://hz.cqqwz.cn/gtmzqxkxdm.html

time ./run.sh
来源：http://hz.kuanghao11.cn/gtzkaeizjj.html

================================================================================
来源：http://hz.zhijiandao.cn/gttsivoqax.html

S. C / C++ 专题
来源：http://hz.mhx1999.top/gtbznyxrvk.html

================================================================================
来源：http://hz.tian-w.cn/gtkxobxrjp.html

[S01] C：Hello World
来源：http://hz.jqgfzy.top/gtmemkbsyv.html

#include <stdio.h>
来源：http://hz.ydzc1.top/gtemfoyrrj.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.sysykeji.top/gtdgggtfvr.html

[S02] C：变量与格式化输出
来源：http://hz.yvedp.cn/gtzgvcxydb.html

int a = 10; printf("%d\n", a);
来源：http://hz.cucudq.cn/gtginbakcx.html

[S03] C：读入整数
来源：http://hz.shanyushiyangtech.top/gtryesaqne.html

int x; scanf("%d", &x);
来源：http://hz.tianlin.xyz/gtfkhznpzc.html

[S04] C：字符串复制
来源：http://hz.shzxlz.cn/gtnhcgwnyq.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.xylfe.cn/gtvybafdzb.html

[S05] C：字符串长度
来源：http://hz.jqgfzy.top/gtkvhwasfa.html

strlen(s)
来源：http://hz.52xcode.cn/gtwrwibuvg.html

[S06] C：字符串比较
来源：http://hz.aibaodan.cn/gtclruxjdf.html

strcmp(a, b) == 0
来源：http://hz.shanyushiyangtech.top/gtdudkqxny.html

[S07] C：数组遍历求和
来源：http://hz.snrcjt.cn/gtannxulnr.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.hfpthk.cn/gtgeuhptij.html

[S08] C：动态内存分配与释放
来源：http://hz.ivvv.top/gtajycfwuk.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.yangfankeji.com/gtlvkqglxt.html

[S09] C：结构体定义与初始化
来源：http://hz.mhx1999.top/gthotqceck.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.gzhubu.top/gtpnarwqzu.html

[S10] C：指针与解引用
来源：http://hz.yj20258.top/gtfwmjdlaa.html

int *p = &a;  *p = 5;
来源：http://hz.aizwys.cn/gtdyxvfwnw.html

[S11] C：逐行读文件
来源：http://hz.zhaomingkeji.xyz/gtgawrszjw.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.hnqzz.top/gtswtdbtpu.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.ywan-chungtsiang.top/gtvbgvzfpw.html

fclose(f);
来源：http://hz.jlsjyb.cn/gtytxffhrf.html

[S12] C：写文件
来源：http://hz.52xcode.cn/gtdugilyhm.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.yueranfly.top/gtakuejynv.html

[S13] C：宏定义
来源：http://hz.316326.xyz/gtxdlmdxbk.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.ybcxt.top/gtbbykuygi.html

[S14] C：枚举
来源：http://hz.ehwqpu.com/gtlnwdbgsy.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.fengsongda.top/gtbqzcczad.html

[S15] C：类型转换
来源：http://hz.ehwqpu.com/gtggwfrqwb.html

(double) a / b
来源：http://hz.zycfv.cn/gtrwsmcrii.html

[S16] C：位操作置位
来源：http://hz.quarkkingdee.top/gtjapudugg.html

x |= (1 << 3);
来源：http://hz.sweek.top/gttjjvvnnu.html

[S17] C：安全拼接字符串
来源：http://hz.nwbrower.top/gtiawgjskt.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.jqgfzy.top/gtwitacgqm.html

[S18] C：命令行参数
来源：http://hz.gzhubu.top/gtjqmptgwg.html

int main(int argc, char **argv)
来源：http://hz.jianghu66.top/gtqjuzpxuj.html

[S19] C：快速排序
来源：http://hz.ehwqpu.com/gtvvovlxdv.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.kuanghao11.cn/gtazidfghq.html

[S20] C：二分查找
来源：http://hz.xinyue.icu/gtjzcvvnkt.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.0kj1m.cn/gtycagwqjf.html

[S21] C：字符类别判断
来源：http://hz.yueranfly.top/gtpzrkzctp.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.pengpengdd.cyou/gtcsthlqau.html

[S22] C：字符串转数字
来源：http://hz.nanxuanxn.top/gtuuyulbgg.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.ybcxt.top/gtollotetw.html

[S23] C：随机数
来源：http://hz.jqgufenzy.top/gthlkqpppa.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.guowangkeji.top/gtgwcxaypn.html

[S24] C：获取本地时间
来源：http://hz.aizwys.cn/gtdhdnocgo.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.yj20258888.top/gtlqwuyopt.html

[S25] C：内存拷贝
来源：http://hz.dashuyun.cn/gteceaejjz.html

memcpy(dst, src, n);
来源：http://hz.9152youxi.cn/gtpgffylbp.html

[S26] C：内存清零
来源：http://hz.sufxvd.cn/gtjczsimsy.html


<!-- 参考信息 -->