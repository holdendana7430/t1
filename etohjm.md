代发 wailian999

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.hammf.cn/gtmlxpaerc.html

[Q54] 清空表
来源：http://hz.ydzc1.top/gttldttiay.html

TRUNCATE TABLE logs;
来源：http://hz.dashuyun.cn/gtxcrpavtb.html

[Q55] 排名（并列占位）
来源：http://hz.mhx1999.top/gtptltoyzg.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.tian-w.cn/gttewkmwbo.html

[Q56] 密集排名（并列不占位）
来源：http://hz.ppjwa.cn/gtwvdospjv.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.birdmap.top/gtxrqbnyvf.html

[Q57] 行号
来源：http://hz.52xcode.cn/gthtlgeabz.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.316326.xyz/gtvegnekcw.html

[Q58] 累计求和
来源：http://hz.yueranfly.top/gtarmlsrms.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.hfpthk.cn/gtngqqpopm.html

[Q59] 分组内累计
来源：http://hz.ppjwa.cn/gtdfozwawc.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.havefunace.top/gtjrsnbyyc.html

[Q60] 取上一行 / 下一行
来源：http://hz.xinyue.icu/gtgnbifrpi.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.xuanzx.com/gtvdaindmz.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.dianchejie.cn/gtjsqmmyxy.html

[Q61] 移动平均
来源：http://hz.tian-w.cn/gtsgkffnqz.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.yuanzhike.top/gtxlzfdqyv.html

[Q62] 分组占比
来源：http://hz.snrcjt.cn/gtrvjhzflf.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.birdmap.top/gtcudjtvit.html

[Q63] 开启事务
来源：http://hz.jinqigufen.top/gtcbgrldyq.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.cucudq.cn/gtxpnfpzcs.html

[Q64] 提交事务
来源：http://hz.shangyingyoupin.top/gtazioxwtf.html

COMMIT;
来源：http://hz.yonumen.top/gtiekjzgqm.html

[Q65] 回滚事务
来源：http://hz.nwbrower.top/gtsqbmohmk.html

ROLLBACK;
来源：http://hz.tanke756.top/gtgcddotci.html

[Q66] 行锁查询
来源：http://hz.sufxvd.cn/gtqzgziwhu.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.jlsjyb.cn/gtoslgquni.html

[Q67] 设置隔离级别
来源：http://hz.xingfuxueyuan.xyz/gthsovltwe.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.meibo888.top/gtdvrpucsp.html

[Q68] 保存点
来源：http://hz.ydjk.org.cn/gtawqnnbqe.html

SAVEPOINT sp1;
来源：http://hz.birdmap.top/gthhxoqsjg.html

ROLLBACK TO sp1;
来源：http://hz.yueranfly.top/gtsyfyudpg.html

[Q69] 查看执行计划
来源：http://hz.ybcxt.top/gtomssgima.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.hfpthk.cn/gtqhanfeaq.html

[Q70] 更新统计信息
来源：http://hz.yangfankeji.com/gtchwabdma.html

ANALYZE TABLE users;
来源：http://hz.yueranfly.top/gtjxbdtslj.html

[Q71] 查看建表语句
来源：http://hz.hysaishi.cn/gtomfjcedr.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.xuetiantiany.cn/gtoxxrzzmv.html

[Q72] 查看索引
来源：http://hz.fengsongda.top/gtsaqxmtuq.html

SHOW INDEX FROM users;
来源：http://hz.vqdsnc.cn/gtyiqhxgeo.html

[Q73] 查看表状态
来源：http://hz.hysaishi.cn/gtyfrhekwk.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.zycfv.cn/gtvluphurx.html

[Q74] 强制使用索引
来源：http://hz.wangdashe.top/gthjzckdle.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.hongshengwenyu.top/gtboiagbea.html

[Q75] 日期格式化
来源：http://hz.cdnleiting.top/gtifmpewiy.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.bjfxy.top/gtiywrztam.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.guowangkeji.top/gtrrjfhnmy.html

[Q76] 按天统计
来源：http://hz.daxiang520.top/gtpprunpos.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.jinyuanbaomall.cn/gtowpvzsel.html

[Q77] 时间加减
来源：http://hz.yj20258.top/gtlxsrpfbh.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.shanyushiyangkeji.top/gtzgruuovm.html

[Q78] 当前时间
来源：http://hz.meibo888.top/gtmocdapuf.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.hnqzz.top/gtmbvtruwh.html

[Q79] 字符串拼接
来源：http://hz.sysykeji.top/gtnouewgfu.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.fengsongda.top/gthidemzsj.html

[Q80] 字符串截取
来源：http://hz.jqgufenzy.top/gtjbaoerpf.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.shanyushiyangkeji.top/gtygvbfgxw.html

[Q81] 字符串替换
来源：http://hz.52xcode.cn/gtcgftphwh.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.quarkkingdee.top/gtrkvfnxhn.html

[Q82] 字符长度与字节长度
来源：http://hz.cucudq.cn/gterpqmggs.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.hywenlv.cn/gtwnqgnwmi.html

[Q83] 大小写转换
来源：http://hz.yongpay.top/gtsbvxpwwv.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.pycfn.com/gtpldumozd.html

[Q84] 去除首尾空格
来源：http://hz.yvedp.cn/gtzouznqcc.html

SELECT TRIM(name) FROM users;
来源：http://hz.sweek.top/gtpjxbunvi.html

[Q85] 数值取整
来源：http://hz.hfpthk.cn/gtjjmmqbui.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.zhaomingkeji.xyz/gtqorlosxx.html

[Q86] 读取 JSON 字段
来源：http://hz.jqgufenzy.top/gtkkjzrudt.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.aibaodan.cn/gtinqrqxik.html

[Q87] JSON 字段做条件
来源：http://hz.daxiang520.top/gtzfjabkbt.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.birdmap.top/gtbycjavlb.html

[Q88] 行转列（条件聚合）
来源：http://hz.jinqigfzy.top/gtyzgxztsu.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.ywan-chungtsiang.top/gtnxwzjygw.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.wangdashe.top/gtmwtgddhv.html

[Q89] 判断表是否存在
来源：http://hz.ehwqpu.com/gtpdrzmwpr.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.haohaochexian.top/gtivzjeymo.html

[Q90] 生成序号列
来源：http://hz.zhengqikj.top/gtjjyxazye.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.yongpay.top/gtpfswyoby.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtmruuvjas.html

R. Bash 专题
来源：http://hz.tian-w.cn/gtihppodcs.html

================================================================================
来源：http://hz.gaohongyu789.top/gtzodwtgnk.html

[R01] shebang 与严格模式
来源：http://hz.yangfankeji.com/gtcniiopkf.html

#!/usr/bin/env bash
来源：http://hz.hnxiangtu.top/gtkwjkkrts.html

set -euo pipefail
来源：http://hz.kuanghao11.cn/gtpixarxvs.html

[R02] 变量赋值与使用
来源：http://hz.tian-w.cn/gtxmelqwud.html

name="Tom"; echo "$name"
来源：http://hz.zdqjudy.top/gtsdmfewkk.html

[R03] 只读变量
来源：http://hz.ivvv.top/gtykhogang.html

readonly PI=3.14
来源：http://hz.bjfxy.top/gtyompwqvv.html

[R04] 位置参数
来源：http://hz.yuanzhike.top/gtqyqkzkkn.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.yanxiufei.cn/gtybztvtkd.html

[R05] 参数默认值
来源：http://hz.jyoumei.cn/gtrhyhlkff.html

name="${1:-default}"
来源：http://hz.daxiang520.top/gtammaoual.html

[R06] 判断命令是否存在
来源：http://hz.xziqi.cn/gtqhfknbdz.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.jinyuanbaomall.cn/gtpchvqyjw.html

[R07] if 判断文件
来源：http://hz.cheryme.top/gtryugeqkq.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.vqdsnc.cn/gtxnfsbzyq.html

[R08] 数值比较
来源：http://hz.9152youxi.cn/gtgigbcgvf.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.wangshuangyany.cn/gtjmfzmpis.html

[R09] 字符串比较
来源：http://hz.shangyingyoupin.top/gtlindhghm.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.dashuyun.cn/gthiarauwx.html

[R10] 正则匹配
来源：http://hz.ehwqpu.com/gtrkpgekku.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.ehwqpu.com/gtoutlanlb.html

[R11] case 多分支
来源：http://hz.52xcode.cn/gtftkwzrzh.html

case "$1" in
来源：http://hz.xingfuxueyuan.xyz/gteguguerr.html

start) echo "启动" ;;
来源：http://hz.yvedp.cn/gtwrrkwopv.html

stop)  echo "停止" ;;
来源：http://hz.jqgufenzy.top/gtlkugyvmn.html

*)     echo "未知命令" ;;
来源：http://hz.c1oappe.top/gtypnrrler.html

esac
来源：http://hz.wangshuangyany.cn/gtgnvkbpow.html

[R12] for 遍历文件
来源：http://hz.jlsjyb.cn/gtsaxdieoi.html

for f in *.txt; do echo "$f"; done
来源：http://hz.jyoumei.cn/gttszengbx.html

[R13] for 计数循环
来源：http://hz.hnqzz.top/gtipjhjkem.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.jiagoushi.top/gtmdwsxvox.html

[R14] C 风格 for
来源：http://hz.quarkkingdee.top/gtecvhojib.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.xuanzx.com/gtwgliqrog.html

[R15] while 逐行读文件
来源：http://hz.yueranfly.top/gtsyixboug.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.feifeiyinyue.top/gtwgdeialh.html

[R16] until 等待条件
来源：http://hz.hnqzz.top/gtidfwsdwl.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.wangdashe.top/gtdmaccfyb.html

[R17] 数组定义与取值
来源：http://hz.shangyingyoupin.top/gtzyxvdxtv.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.jinghuilouyu.cn/gtugcfdroc.html

[R18] 遍历数组
来源：http://hz.hywenlv.cn/gtretrilme.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.yonumen.top/gtssmmdthw.html

[R19] 数组长度
来源：http://hz.jiagoushi.top/gtafqemvwl.html

echo "${#arr[@]}"
来源：http://hz.ppjwa.cn/gtzdfdzasd.html

[R20] 关联数组（字典）
来源：http://hz.bjfxy.top/gtnfbidypf.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.tian-w.cn/gtmrmjjpfs.html

[R21] 字符串长度
来源：http://hz.zhixingplan.top/gtwyhmzrza.html

echo "${#s}"
来源：http://hz.vqdsnc.cn/gtpwsuithw.html

[R22] 截取子串
来源：http://hz.yj20258.top/gttzvumhln.html

echo "${s:0:5}"
来源：http://hz.shangyingyoupin.top/gtplkovexc.html

[R23] 字符串替换
来源：http://hz.birdmap.top/gtikvfgmrg.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.cqqwz.cn/gtdfadjwpe.html

[R24] 大小写转换
来源：http://hz.birdmap.top/gtwpocpaqz.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.guowangkeji.top/gtamyqafxl.html

[R25] 去后缀 / 去前缀
来源：http://hz.hysaishi.cn/gtmxwilxzr.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.xylfe.cn/gtfjscoysv.html

[R26] 命令替换
来源：http://hz.jinqigufen.top/gtctuznbcr.html

now=$(date +%F); echo "$now"
来源：http://hz.fengsongda.top/gtmhxujaxk.html

[R27] 算术展开
来源：http://hz.hammf.cn/gtrhvcryrh.html

echo $((1 + 2 * 3))
来源：http://hz.mhx1999.top/gtlwydmvke.html

[R28] 浮点运算
来源：http://hz.pengpengdd.cyou/gttlpqowro.html

echo "scale=2; 10/3" | bc
来源：http://hz.yanxiufei.cn/gtgqewpwqe.html

[R29] 定义函数
来源：http://hz.zhoulong.xyz/gtmfopjeze.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.shzxlz.cn/gtxkbqvjyi.html

[R30] 函数返回状态码
来源：http://hz.316326.xyz/gtwiezwbyl.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.jqgfzy.top/gtricoxogf.html

[R31] 局部变量
来源：http://hz.hnqzz.top/gtfrpwften.html

f() { local x=1; echo "$x"; }
来源：http://hz.xylfe.cn/gtbzqzzbzy.html

[R32] 参数个数校验
来源：http://hz.aibaodan.cn/gtvhrgpbsl.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.jyoumei.cn/gtqwftwyzx.html

[R33] 捕获错误并提示行号
来源：http://hz.sweek.top/gtjorcqzmy.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.yj20258.top/gtthmffczw.html

[R34] 退出时清理
来源：http://hz.shanyushiyangtech.top/gthnlgfpwh.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.tanke756.top/gtlzcdwebk.html

[R35] 后台执行并等待
来源：http://hz.wangshuangyany.cn/gtevrenhoz.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.smart0.xyz/gtvpwkqnzc.html

[R36] 并发执行多个任务
来源：http://hz.daxiang520.top/gtsvwmtxik.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.hfpthk.cn/gtxmdpeciw.html

[R37] 把输出赋给变量
来源：http://hz.yanxiufei.cn/gtnperlrdn.html

files=$(ls -1)
来源：http://hz.c1oappe.top/gtonxoaluu.html

[R38] 管道串联
来源：http://hz.wangdashe.top/gtdibuccyq.html

cat a.txt | grep -i error | wc -l
来源：http://hz.jinghuilouyu.cn/gtqbsgwkqf.html

[R39] 重定向标准输出与错误
来源：http://hz.meibo888.top/gtadrzkhuo.html

cmd > out.log 2>&1
来源：http://hz.aizwys.cn/gthzlxeckm.html

[R40] 追加写日志
来源：http://hz.jyoumei.cn/gtzegwynye.html

echo "log" >> out.log
来源：http://hz.jinghuilouyu.cn/gtxmffbsps.html

[R41] 丢弃输出
来源：http://hz.gogol.net.cn/gtdgmbindk.html

cmd >/dev/null 2>&1
来源：http://hz.ywan-chungtsiang.top/gtenuorery.html

[R42] 输入重定向
来源：http://hz.sufxvd.cn/gtecotljcz.html

wc -l < a.txt
来源：http://hz.meibo888.top/gtxxfdbtga.html

[R43] 按名字查找文件
来源：http://hz.gaohongyu789.top/gtzfsjysua.html

find . -name "*.log" -type f
来源：http://hz.xylfe.cn/gtkfeaqsgt.html

[R44] 按修改时间查找
来源：http://hz.tanke756.top/gthyfamnld.html

find . -mtime -7 -type f
来源：http://hz.cheryme.top/gtxymfyfxd.html

[R45] 批量删除
来源：http://hz.guannengcc.top/gtgbmicxgw.html

find . -name "*.tmp" -delete
来源：http://hz.shzxlz.cn/gtfrpvayjp.html

[R46] 递归替换文件内容
来源：http://hz.guannengcc.top/gtbnhrfgfm.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.yueranfly.top/gtcbjmoprv.html

[R47] sed 单行替换
来源：http://hz.iojbl.cn/gtpqljuacd.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.jyoumei.cn/gtsxdwevss.html

[R48] awk 取指定列
来源：http://hz.hysaishi.cn/gtemekvdwx.html

awk '{print $1, $3}' a.txt
来源：http://hz.nanxuanxn.top/gtktomzlwi.html

[R49] awk 带条件
来源：http://hz.yongpay.top/gtoqqaljuw.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.mhx1999.top/gtvkkdulit.html

[R50] awk 求和
来源：http://hz.zhongyouzk.top/gtgaedbwfy.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.havefunace.top/gtaydmxeoi.html

[R51] 排序去重取前几
来源：http://hz.jlsjyb.cn/gtgrubhtpk.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.nwbrower.top/gtpqpgbvfe.html

[R52] 统计行数
来源：http://hz.cdnleiting.top/gtelftsizx.html

wc -l a.txt
来源：http://hz.daria6918.cn/gtoiczvtdb.html

[R53] 查看文件头与实时尾
来源：http://hz.daxiang520.top/gtllncyupe.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.0kj1m.cn/gtawbsansl.html

[R54] 比较两个文件
来源：http://hz.sweek.top/gtfetfxcym.html

diff a.txt b.txt
来源：http://hz.yanxiufei.cn/gtmdqejfgp.html

[R55] 压缩与解压
来源：http://hz.guowangkeji.top/gtfsohfahy.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.jqgfzy.top/gtmtdlvhgn.html

[R56] 远程拷贝
来源：http://hz.yvedp.cn/gtpwmsgogt.html

scp file user@host:/path/
来源：http://hz.hfpthk.cn/gtwdjwtlxz.html

[R57] 远程执行命令
来源：http://hz.jqgufenzy.top/gtmocdoeaa.html

ssh user@host 'uptime'
来源：http://hz.sufxvd.cn/gtovczycfc.html

[R58] 下载文件
来源：http://hz.wangdashe.top/gtpmcstngg.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.daria6918.cn/gtavfjgudl.html

[R59] 发 POST JSON
来源：http://hz.gaohongyu789.top/gtnnxtgheq.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.jyoumei.cn/gtxsodstxc.html

[R60] 只看 HTTP 状态码
来源：http://hz.jlsjyb.cn/gtcapmvumh.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.mhx1999.top/gtcmellifc.html

[R61] 磁盘占用
来源：http://hz.cdnleiting.top/gtzoiotqja.html

df -h;  du -sh *
来源：http://hz.yangfankeji.com/gtvxugzbhy.html

[R62] 找最占空间的文件
来源：http://hz.nanxinkj.top/gtnrrbogca.html

du -ah . | sort -rh | head -10
来源：http://hz.zhaomingkeji.xyz/gtkqpkcejg.html

[R63] 内存与进程
来源：http://hz.dashuyun.cn/gthcjvfoes.html

free -h;  ps aux | grep nginx
来源：http://hz.shanyushiyangkeji.top/gtwpjqzspf.html

[R64] 结束进程
来源：http://hz.zhengqikj.top/gtyroxsdag.html

kill -9 $(pgrep -f app.py)
来源：http://hz.hnqzz.top/gtjsxpurmy.html

[R65] 查看端口占用
来源：http://hz.cqqwz.cn/gtibqbgpoz.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.52xcode.cn/gtzclrzlfo.html

[R66] 定时任务
来源：http://hz.jlsjyb.cn/gthousglyo.html

crontab -e;  crontab -l
来源：http://hz.c1oappe.top/gtezogpriu.html

[R67] 生成随机十六进制串
来源：http://hz.ivvv.top/gtijsudzls.html

openssl rand -hex 16
来源：http://hz.svipenyu.cn/gtfvbtlyzm.html

[R68] 计算文件校验值
来源：http://hz.yangfankeji.com/gtjszpkmgt.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.yonumen.top/gtsabixedf.html

[R69] 生成随机密码
来源：http://hz.0kj1m.cn/gtjaeejidy.html

head -c 16 /dev/urandom | base64
来源：http://hz.feifeiyinyue.top/gtkjsmovhj.html

[R70] 时间戳与互转
来源：http://hz.zdqjudy.top/gtwqkznvpl.html

date +%s;  date -d @1700000000
来源：http://hz.gotoacloud.top/gthucuaxwq.html

[R71] 日期格式化
来源：http://hz.gotoacloud.top/gtihvvpyos.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.wangshuangyany.cn/gtxynurlzy.html

[R72] 等待端口就绪
来源：http://hz.guowangkeji.top/gthuedtcix.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.xziqi.cn/gtjlpprvla.html

[R73] 分割大日志
来源：http://hz.nanxuanxn.top/gtkgftbjgw.html

split -l 1000 big.log part_
来源：http://hz.aibaodan.cn/gtgdlvyeas.html

[R74] 批量重命名
来源：http://hz.fengsongda.top/gtkyizizvb.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.fengsongda.top/gtfcsywqjm.html

[R75] 导出环境变量
来源：http://hz.jianghu66.top/gtpglzhftf.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.shzxlz.cn/gtdswxqqml.html

[R76] 使用临时文件
来源：http://hz.sysykeji.top/gtupxqrnih.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.9152youxi.cn/gtutdqxsqs.html

[R77] 读取用户输入
来源：http://hz.quarkkingdee.top/gtivmieklj.html

read -rp "请输入: " ans
来源：http://hz.feifeiyinyue.top/gtmbtctquf.html

[R78] 交互式菜单
来源：http://hz.fengsongda.top/gtjzcocmam.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.tanke756.top/gtrpzsxwwc.html

[R79] 解析命令行选项
来源：http://hz.xingfuxueyuan.xyz/gtkrmnpfit.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.fengsongda.top/gttsocncjy.html

[R80] 查看脚本执行耗时
来源：http://hz.zhaomingkeji.xyz/gtojeufjwa.html

time ./run.sh
来源：http://hz.jinqigfzy.top/gtyqlbsmon.html

================================================================================
来源：http://hz.jiagoushi.top/gtirqdgegb.html

S. C / C++ 专题
来源：http://hz.zhijiandao.cn/gtsmckmmxc.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtlyhexask.html

[S01] C：Hello World
来源：http://hz.sxryk.cn/gtypzlvrzv.html

#include <stdio.h>
来源：http://hz.hysaishi.cn/gtovcjcrku.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.sweek.top/gtyobejwka.html

[S02] C：变量与格式化输出
来源：http://hz.ydzc1.top/gtidrhvqzu.html

int a = 10; printf("%d\n", a);
来源：http://hz.sysykeji.top/gtzgkezewi.html

[S03] C：读入整数
来源：http://hz.zhixingplan.top/gtercfrcxv.html

int x; scanf("%d", &x);
来源：http://hz.feifeiyinyue.top/gtbggjunbv.html

[S04] C：字符串复制
来源：http://hz.sysykeji.top/gthhfspehp.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.nwbrower.top/gtaysqumup.html

[S05] C：字符串长度
来源：http://hz.52xcode.cn/gtzrgjzykg.html

strlen(s)
来源：http://hz.jianghu66.top/gtiaylhqne.html

[S06] C：字符串比较
来源：http://hz.jqgufenzy.top/gtpyvjnsqk.html

strcmp(a, b) == 0
来源：http://hz.gzhubu.top/gtudsgdxwi.html

[S07] C：数组遍历求和
来源：http://hz.zhijiandao.cn/gtgkunsqml.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.yueranfly.top/gthrhfcdcw.html

[S08] C：动态内存分配与释放
来源：http://hz.0kj1m.cn/gtrrviudui.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.yuxming.cn/gtqjvddnpm.html

[S09] C：结构体定义与初始化
来源：http://hz.gzhubu.top/gtjhlradlp.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.sxryk.cn/gtbvoosupc.html

[S10] C：指针与解引用
来源：http://hz.birdmap.top/gtktacnrzn.html

int *p = &a;  *p = 5;
来源：http://hz.gaohongyu789.top/gtwbnwtvjy.html

[S11] C：逐行读文件
来源：http://hz.hywenlv.cn/gtjuyfanws.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.tian-w.cn/gtcowntjeq.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.ydzc1.top/gtfxapvcod.html

fclose(f);
来源：http://hz.316326.xyz/gtwhbxbdat.html

[S12] C：写文件
来源：http://hz.shuidangran.top/gtovebifuc.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.hysaishi.cn/gtuytoshtr.html

[S13] C：宏定义
来源：http://hz.vqdsnc.cn/gtgkfxznxj.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.aizwys.cn/gtvjmmuhlb.html

[S14] C：枚举
来源：http://hz.aizwys.cn/gtcqknwlbm.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.zhongyouzk.top/gtcouqglor.html

[S15] C：类型转换
来源：http://hz.jinyuanbaomall.cn/gtezagolgt.html

(double) a / b
来源：http://hz.birdmap.top/gtkeaszuwy.html

[S16] C：位操作置位
来源：http://hz.yueranfly.top/gtvyvwdyzd.html

x |= (1 << 3);
来源：http://hz.cqqwz.cn/gtvetieqds.html

[S17] C：安全拼接字符串
来源：http://hz.shuidangran.top/gtfvcezxup.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.yonumen.top/gtbyaqgzyj.html

[S18] C：命令行参数
来源：http://hz.aibaodan.cn/gtutteunyn.html

int main(int argc, char **argv)
来源：http://hz.xinyue.icu/gticuooopx.html

[S19] C：快速排序
来源：http://hz.aizwys.cn/gtfehohydq.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.gzhubu.top/gttbxwwgcs.html

[S20] C：二分查找
来源：http://hz.pycfn.com/gthumtthou.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.jinyuanbaomall.cn/gtmuetidsz.html

[S21] C：字符类别判断
来源：http://hz.jiagoushi.top/gtldmyxheq.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.nanxinkj.top/gtiojihvkb.html

[S22] C：字符串转数字
来源：http://hz.jinqigfzy.top/gtusdikvat.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.yvedp.cn/gtjuoyeivu.html

[S23] C：随机数
来源：http://hz.kuanghao11.cn/gtaualxwrt.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.c1oappe.top/gtmkqhbgxo.html

[S24] C：获取本地时间
来源：http://hz.jinyuanbaomall.cn/gtqdxfermv.html


<!-- 参考信息 -->