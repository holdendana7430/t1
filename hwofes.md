代发 wailian999

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.zhengqikj.top/gtrkbenlzu.html

[Q56] 密集排名（并列不占位）
来源：http://hz.hongshengwenyu.top/gtqyoelgys.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.yanxiufei.cn/gttmviermx.html

[Q57] 行号
来源：http://hz.fzhhl.top/gtablohftd.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.bjfxy.top/gtiwbpvbbu.html

[Q58] 累计求和
来源：http://hz.yvedp.cn/gtmfrjwsxn.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.mhx1999.top/gtclhndknw.html

[Q59] 分组内累计
来源：http://hz.316326.xyz/gtyyzsqnek.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.zycfv.cn/gtkrqxwuwb.html

[Q60] 取上一行 / 下一行
来源：http://hz.zhixingplan.top/gtypyssvmj.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.shzxlz.cn/gtyfpnxtpd.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.vqdsnc.cn/gtpewvchve.html

[Q61] 移动平均
来源：http://hz.fzhhl.top/gtwfokysgt.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.hywenlv.cn/gtkboxkgde.html

[Q62] 分组占比
来源：http://hz.havefunace.top/gtngmccavw.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.cheryme.top/gtczaysooy.html

[Q63] 开启事务
来源：http://hz.hysaishi.cn/gtfckboafe.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.xuetiantiany.cn/gtvlykjmta.html

[Q64] 提交事务
来源：http://hz.9152youxi.cn/gtpogelvfd.html

COMMIT;
来源：http://hz.smart0.xyz/gtinjugmsj.html

[Q65] 回滚事务
来源：http://hz.ybcxt.top/gtaxebgixh.html

ROLLBACK;
来源：http://hz.daria6918.cn/gtxdwccnhy.html

[Q66] 行锁查询
来源：http://hz.nanxuanxn.top/gtlltbrsiz.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.xylfe.cn/gtczqcdmmf.html

[Q67] 设置隔离级别
来源：http://hz.xuetiantiany.cn/gtoxgzqkkw.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.andypj.xyz/gthjxzqurn.html

[Q68] 保存点
来源：http://hz.9152youxi.cn/gtyuaahkte.html

SAVEPOINT sp1;
来源：http://hz.sxryk.cn/gtcqwdmeqv.html

ROLLBACK TO sp1;
来源：http://hz.birdmap.top/gtfuulkyoc.html

[Q69] 查看执行计划
来源：http://hz.ivvv.top/gttkqnjvol.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.aizwys.cn/gtuqevmqao.html

[Q70] 更新统计信息
来源：http://hz.yongpay.top/gtkypmelkh.html

ANALYZE TABLE users;
来源：http://hz.hongshengwenyu.top/gtfqdghudo.html

[Q71] 查看建表语句
来源：http://hz.cheryme.top/gtauimoqse.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.daria6918.cn/gtmnydbufa.html

[Q72] 查看索引
来源：http://hz.xinyue.icu/gtgqrldwzl.html

SHOW INDEX FROM users;
来源：http://hz.gogol.net.cn/gtmyqbhqfd.html

[Q73] 查看表状态
来源：http://hz.hnxiangtu.top/gtowoeogol.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.jqgufenzy.top/gtcpkaazkp.html

[Q74] 强制使用索引
来源：http://hz.yangfankeji.com/gtdsdjqgsa.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.52xcode.cn/gtmgagglfu.html

[Q75] 日期格式化
来源：http://hz.jqgfzy.top/gtwtjexied.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.xuetiantiany.cn/gtedzzsywa.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.tianlin.xyz/gtauhimfrh.html

[Q76] 按天统计
来源：http://hz.yanxiufei.cn/gtfguwfusf.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.shanyushiyangtech.top/gtdxtuapgu.html

[Q77] 时间加减
来源：http://hz.tianlin.xyz/gtrilxiked.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.ydzc1.top/gtzvhxauhv.html

[Q78] 当前时间
来源：http://hz.svipenyu.cn/gtdbwkgxnv.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.jinghuilouyu.cn/gtkfcgidhz.html

[Q79] 字符串拼接
来源：http://hz.daxiang520.top/gtxyjkvayn.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.shanyushiyangkeji.top/gtirzoegbo.html

[Q80] 字符串截取
来源：http://hz.yj20258.top/gttwwouyqs.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.zhiwuduotai.top/gtxgurohje.html

[Q81] 字符串替换
来源：http://hz.fengsongda.top/gtttqohodh.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.52xcode.cn/gticgglrvs.html

[Q82] 字符长度与字节长度
来源：http://hz.yj20258.top/gtlrmpubxb.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.ybcxt.top/gthespowwc.html

[Q83] 大小写转换
来源：http://hz.dashuyun.cn/gtxaaowapf.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.52xcode.cn/gtxaqmsawj.html

[Q84] 去除首尾空格
来源：http://hz.wangdashe.top/gtsjlfxzzr.html

SELECT TRIM(name) FROM users;
来源：http://hz.ppjwa.cn/gtojbmzcwf.html

[Q85] 数值取整
来源：http://hz.xuanzx.com/gtehkffshu.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.yj202588.top/gtrxjidpuq.html

[Q86] 读取 JSON 字段
来源：http://hz.cheryme.top/gtvpnvtruv.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.316326.xyz/gtjymtyvkp.html

[Q87] JSON 字段做条件
来源：http://hz.hongshengwenyu.top/gtmarsauiv.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.xingfuxueyuan.xyz/gteipgzxbo.html

[Q88] 行转列（条件聚合）
来源：http://hz.mhx1999.top/gtppesuzai.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.jianghu66.top/gtheweuyvh.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.chenlongwang.top/gtpyviduza.html

[Q89] 判断表是否存在
来源：http://hz.cucudq.cn/gtfcybkbdb.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.chenjidiqi.icu/gtakdnysjo.html

[Q90] 生成序号列
来源：http://hz.zhoulong.xyz/gtvlnqgehq.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.fzhhl.top/gtjmytifsd.html

================================================================================
来源：http://hz.yvedp.cn/gtqvfibxrv.html

R. Bash 专题
来源：http://hz.xylfe.cn/gtjcuttefb.html

================================================================================
来源：http://hz.zhongyouzk.top/gtvqjdwcss.html

[R01] shebang 与严格模式
来源：http://hz.jqgufenzy.top/gtqvshjkmt.html

#!/usr/bin/env bash
来源：http://hz.fzhhl.top/gtamujenib.html

set -euo pipefail
来源：http://hz.gaohongyu789.top/gtncxxajdl.html

[R02] 变量赋值与使用
来源：http://hz.c1oappe.top/gtjmdflvxt.html

name="Tom"; echo "$name"
来源：http://hz.jinqigfzy.top/gtplguvszt.html

[R03] 只读变量
来源：http://hz.xinyue.icu/gtidemwlus.html

readonly PI=3.14
来源：http://hz.haohaochexian.top/gtaknaanck.html

[R04] 位置参数
来源：http://hz.dashuyun.cn/gtzevoprqi.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.xuetiantiany.cn/gtxbbsasao.html

[R05] 参数默认值
来源：http://hz.meibo888.top/gtjonvjglo.html

name="${1:-default}"
来源：http://hz.yongpay.top/gtdgdoungt.html

[R06] 判断命令是否存在
来源：http://hz.daxiang520.top/gtdnhmczrh.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.hysaishi.cn/gtknoddaxu.html

[R07] if 判断文件
来源：http://hz.ybcxt.top/gttkookizm.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.shzxlz.cn/gtbizdsjgz.html

[R08] 数值比较
来源：http://hz.shangyingyoupin.top/gthfpixusm.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.jqgufenzy.top/gtzyllffog.html

[R09] 字符串比较
来源：http://hz.bjfxy.top/gtxbhwkxtj.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.xinyue.icu/gtvrchtbuq.html

[R10] 正则匹配
来源：http://hz.jqgfzy.top/gtryddrinw.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.jianghu66.top/gtfkwuhfrx.html

[R11] case 多分支
来源：http://hz.jqgfzy.top/gtnuskjpbf.html

case "$1" in
来源：http://hz.guowangkeji.top/gtxebkaqcy.html

start) echo "启动" ;;
来源：http://hz.jiagoushi.top/gtrzummlfa.html

stop)  echo "停止" ;;
来源：http://hz.jlsjyb.cn/gtljwnjzad.html

*)     echo "未知命令" ;;
来源：http://hz.snrcjt.cn/gtnyoqlmfa.html

esac
来源：http://hz.haohaochexian.top/gtafadxfop.html

[R12] for 遍历文件
来源：http://hz.hongshengwenyu.top/gtzzvgzoxu.html

for f in *.txt; do echo "$f"; done
来源：http://hz.ydjk.org.cn/gtswdwcwlo.html

[R13] for 计数循环
来源：http://hz.sufxvd.cn/gtzpcbfczm.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.52xcode.cn/gtmcbgnnyg.html

[R14] C 风格 for
来源：http://hz.jlsjyb.cn/gtdvnlxpev.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.wangshuangyany.cn/gtpoewvsfh.html

[R15] while 逐行读文件
来源：http://hz.0kj1m.cn/gtfxcghaed.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.aizwys.cn/gtrobeoxsc.html

[R16] until 等待条件
来源：http://hz.zycfv.cn/gtfvhvlrgb.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.redwolf501.top/gtzqgdalle.html

[R17] 数组定义与取值
来源：http://hz.gotoacloud.top/gtlqcdamoz.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.jqgufenzy.top/gtlnnncgqr.html

[R18] 遍历数组
来源：http://hz.shangyingyoupin.top/gtkvcenzkk.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.xuetiantiany.cn/gtrvwfggke.html

[R19] 数组长度
来源：http://hz.0kj1m.cn/gtrvgcqsch.html

echo "${#arr[@]}"
来源：http://hz.zhengqikj.top/gtiovrkpyc.html

[R20] 关联数组（字典）
来源：http://hz.pengpengdd.cyou/gtlqrpmbff.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.ydzc1.top/gtoezzagcc.html

[R21] 字符串长度
来源：http://hz.yj20258.top/gtxlimltvz.html

echo "${#s}"
来源：http://hz.yonumen.top/gtasdrlpsq.html

[R22] 截取子串
来源：http://hz.zhengqikj.top/gtxrebegat.html

echo "${s:0:5}"
来源：http://hz.yuxming.cn/gtdbwpfdxe.html

[R23] 字符串替换
来源：http://hz.fengsongda.top/gtglmuemjd.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.chenlongwang.top/gtmprxxjyk.html

[R24] 大小写转换
来源：http://hz.zhiwuduotai.top/gtjyltaboz.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.0kj1m.cn/gtcnhwpifa.html

[R25] 去后缀 / 去前缀
来源：http://hz.ydjk.org.cn/gtgufqxjge.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.jyoumei.cn/gtlgdyusau.html

[R26] 命令替换
来源：http://hz.jiagoushi.top/gtgtzbogyy.html

now=$(date +%F); echo "$now"
来源：http://hz.shuidangran.top/gtvushfzav.html

[R27] 算术展开
来源：http://hz.nanxinkj.top/gtavgxrjof.html

echo $((1 + 2 * 3))
来源：http://hz.meibo888.top/gtgnhgvouf.html

[R28] 浮点运算
来源：http://hz.xinyue.icu/gtroudfycr.html

echo "scale=2; 10/3" | bc
来源：http://hz.yj202588.top/gtdpkqfyfr.html

[R29] 定义函数
来源：http://hz.haohaochexian.top/gtxxygrryk.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.ppjwa.cn/gtkjfasxwz.html

[R30] 函数返回状态码
来源：http://hz.aizwys.cn/gtkahevfsj.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.cheryme.top/gtnedpgjdc.html

[R31] 局部变量
来源：http://hz.cucudq.cn/gtggxqhgkz.html

f() { local x=1; echo "$x"; }
来源：http://hz.yanxiufei.cn/gtezvxqmao.html

[R32] 参数个数校验
来源：http://hz.birdmap.top/gtlvtageak.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.xylfe.cn/gtsdpidexw.html

[R33] 捕获错误并提示行号
来源：http://hz.zdqjudy.top/gtnwvgsfwl.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.yonumen.top/gtmbweqzhl.html

[R34] 退出时清理
来源：http://hz.feifeiyinyue.top/gtfvfcmbwz.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.zycfv.cn/gtxebdwhrm.html

[R35] 后台执行并等待
来源：http://hz.yj20258888.top/gtwhpzqeyd.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.yuanzhike.top/gtjfdmqios.html

[R36] 并发执行多个任务
来源：http://hz.feifeiyinyue.top/gtxbxncubk.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.sufxvd.cn/gtgxilobpu.html

[R37] 把输出赋给变量
来源：http://hz.zhixingplan.top/gtqmvziabb.html

files=$(ls -1)
来源：http://hz.xinyue.icu/gtgrnqwdqy.html

[R38] 管道串联
来源：http://hz.feifeiyinyue.top/gtsytdxhkm.html

cat a.txt | grep -i error | wc -l
来源：http://hz.daxiang520.top/gtvdscqfsd.html

[R39] 重定向标准输出与错误
来源：http://hz.jqgfzy.top/gtwfsyvecg.html

cmd > out.log 2>&1
来源：http://hz.havefunace.top/gtimqpehaq.html

[R40] 追加写日志
来源：http://hz.shzxlz.cn/gtcwkafnhs.html

echo "log" >> out.log
来源：http://hz.hysaishi.cn/gtxflhtcer.html

[R41] 丢弃输出
来源：http://hz.gogol.net.cn/gtpmiofrjq.html

cmd >/dev/null 2>&1
来源：http://hz.yongpay.top/gtprmemyjd.html

[R42] 输入重定向
来源：http://hz.zhongyouzk.top/gtikqbczzj.html

wc -l < a.txt
来源：http://hz.iojbl.cn/gtbbcfzwcy.html

[R43] 按名字查找文件
来源：http://hz.mhx1999.top/gtrtwdscre.html

find . -name "*.log" -type f
来源：http://hz.yvedp.cn/gtfadeimom.html

[R44] 按修改时间查找
来源：http://hz.yangfankeji.com/gtrnbmazts.html

find . -mtime -7 -type f
来源：http://hz.tian-w.cn/gtaoovjxfz.html

[R45] 批量删除
来源：http://hz.ehwqpu.com/gtzgubyzgz.html

find . -name "*.tmp" -delete
来源：http://hz.hammf.cn/gtmbpimoqz.html

[R46] 递归替换文件内容
来源：http://hz.hnxiangtu.top/gthjrmxgql.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.jlsjyb.cn/gtyslzoaxn.html

[R47] sed 单行替换
来源：http://hz.dianchejie.cn/gtkbruubrx.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.xingfuxueyuan.xyz/gtuucnyhze.html

[R48] awk 取指定列
来源：http://hz.xinyue.icu/gtwfwxjaqd.html

awk '{print $1, $3}' a.txt
来源：http://hz.ybcxt.top/gtlyzwfker.html

[R49] awk 带条件
来源：http://hz.yueranfly.top/gtwxsjafaz.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.dashuyun.cn/gtqsdquldu.html

[R50] awk 求和
来源：http://hz.yonumen.top/gttxpcyzmk.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.dashuyun.cn/gtbkqyvlgj.html

[R51] 排序去重取前几
来源：http://hz.sysykeji.top/gtlstybkvp.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.xinyue.icu/gtvvvkuogp.html

[R52] 统计行数
来源：http://hz.chenlongwang.top/gtchufmeso.html

wc -l a.txt
来源：http://hz.nanxuanxn.top/gtwdruzsyi.html

[R53] 查看文件头与实时尾
来源：http://hz.shuidangran.top/gtaxptvvfz.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.jinqigufen.top/gtoxtmianw.html

[R54] 比较两个文件
来源：http://hz.zhengqikj.top/gtacnvrexj.html

diff a.txt b.txt
来源：http://hz.chenlongwang.top/gtrujbebgo.html

[R55] 压缩与解压
来源：http://hz.smart0.xyz/gtupzpuuoh.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.zhongyouzk.top/gtyvsxqtiz.html

[R56] 远程拷贝
来源：http://hz.shuidangran.top/gtdwvhbjal.html

scp file user@host:/path/
来源：http://hz.shanyushiyangtech.top/gtechntvxx.html

[R57] 远程执行命令
来源：http://hz.jlsjyb.cn/gtvyytlfyy.html

ssh user@host 'uptime'
来源：http://hz.jianghu66.top/gtggxhaalh.html

[R58] 下载文件
来源：http://hz.zhengqikj.top/gtojngswtl.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.jinghuilouyu.cn/gtoprvtdof.html

[R59] 发 POST JSON
来源：http://hz.quarkkingdee.top/gthrmpchqf.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.zhixingplan.top/gtpbxakwxe.html

[R60] 只看 HTTP 状态码
来源：http://hz.nanxuanxn.top/gtvlnghxuq.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.52xcode.cn/gtfoexwovh.html

[R61] 磁盘占用
来源：http://hz.guannengcc.top/gtzlrfwcck.html

df -h;  du -sh *
来源：http://hz.hywenlv.cn/gtnbjcmlpf.html

[R62] 找最占空间的文件
来源：http://hz.hongshengwenyu.top/gtdqlbkxli.html

du -ah . | sort -rh | head -10
来源：http://hz.zhijiandao.cn/gtqltwlkec.html

[R63] 内存与进程
来源：http://hz.vqdsnc.cn/gtvrfbyukz.html

free -h;  ps aux | grep nginx
来源：http://hz.gotoacloud.top/gtplyhdaeu.html

[R64] 结束进程
来源：http://hz.ybcxt.top/gttyvwgxgg.html

kill -9 $(pgrep -f app.py)
来源：http://hz.yuxming.cn/gttrbqdrec.html

[R65] 查看端口占用
来源：http://hz.svipenyu.cn/gtrqzeopdz.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.ywan-chungtsiang.top/gtnkphcypp.html

[R66] 定时任务
来源：http://hz.jinqigfzy.top/gtyapevtzw.html

crontab -e;  crontab -l
来源：http://hz.jqgufenzy.top/gtuulrayxg.html

[R67] 生成随机十六进制串
来源：http://hz.gaohongyu789.top/gtkdgujchr.html

openssl rand -hex 16
来源：http://hz.pycfn.com/gtzikcmpti.html

[R68] 计算文件校验值
来源：http://hz.jinyuanbaomall.cn/gtpitjzyxr.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.ywan-chungtsiang.top/gtaidmgoak.html

[R69] 生成随机密码
来源：http://hz.bjfxy.top/gtnsmnqslh.html

head -c 16 /dev/urandom | base64
来源：http://hz.hongshengwenyu.top/gtqdnxiirm.html

[R70] 时间戳与互转
来源：http://hz.aibaodan.cn/gtzvmragag.html

date +%s;  date -d @1700000000
来源：http://hz.pycfn.com/gtihjbkyxw.html

[R71] 日期格式化
来源：http://hz.zhengqikj.top/gtienqtphp.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.jianghu66.top/gtibsjnecu.html

[R72] 等待端口就绪
来源：http://hz.shuidangran.top/gtnoensozr.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.pycfn.com/gtcuqymdsj.html

[R73] 分割大日志
来源：http://hz.svipenyu.cn/gtcvpbvigz.html

split -l 1000 big.log part_
来源：http://hz.sxryk.cn/gthxwctuty.html

[R74] 批量重命名
来源：http://hz.iojbl.cn/gteltabury.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.shzxlz.cn/gtqnofhoow.html

[R75] 导出环境变量
来源：http://hz.shangyingyoupin.top/gtfyhdyrlk.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.52xcode.cn/gtkmgbmzae.html

[R76] 使用临时文件
来源：http://hz.ppjwa.cn/gtyjpfjiux.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.shzxlz.cn/gtzfdehfcd.html

[R77] 读取用户输入
来源：http://hz.aibaodan.cn/gtseikhgng.html

read -rp "请输入: " ans
来源：http://hz.haohaochexian.top/gtvqpikuvi.html

[R78] 交互式菜单
来源：http://hz.xuetiantiany.cn/gtgedgkbdi.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.bjfxy.top/gtiruzuzuw.html

[R79] 解析命令行选项
来源：http://hz.yongpay.top/gtktizfbme.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.aibaodan.cn/gtnggzlppn.html

[R80] 查看脚本执行耗时
来源：http://hz.wangdashe.top/gtkuipjqan.html

time ./run.sh
来源：http://hz.cqqwz.cn/gtnyqmqqpk.html

================================================================================
来源：http://hz.mhx1999.top/gtyveoqyeo.html

S. C / C++ 专题
来源：http://hz.cashguo.top/gtramkiqnc.html

================================================================================
来源：http://hz.yonumen.top/gtmrlciaff.html

[S01] C：Hello World
来源：http://hz.nwbrower.top/gtvifszzop.html

#include <stdio.h>
来源：http://hz.cdnleiting.top/gtqudaupfg.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.yvedp.cn/gtxjmmiyld.html

[S02] C：变量与格式化输出
来源：http://hz.shanyushiyangkeji.top/gtttsarcoh.html

int a = 10; printf("%d\n", a);
来源：http://hz.ybcxt.top/gtbrtzwyow.html

[S03] C：读入整数
来源：http://hz.hysaishi.cn/gtkljvdbvw.html

int x; scanf("%d", &x);
来源：http://hz.xuanzx.com/gtdhruhwjd.html

[S04] C：字符串复制
来源：http://hz.xylfe.cn/gtellifvth.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.shanyushiyangkeji.top/gtuesrxmbh.html

[S05] C：字符串长度
来源：http://hz.xinyue.icu/gtcwledfie.html

strlen(s)
来源：http://hz.sufxvd.cn/gtsvzekxwk.html

[S06] C：字符串比较
来源：http://hz.jinqigufen.top/gtjzqzyldz.html

strcmp(a, b) == 0
来源：http://hz.tianlin.xyz/gtipzgtvdl.html

[S07] C：数组遍历求和
来源：http://hz.xingfuxueyuan.xyz/gtsfipyrvr.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.redwolf501.top/gtjyujdftp.html

[S08] C：动态内存分配与释放
来源：http://hz.shangyingyoupin.top/gthavtrusz.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.jianghu66.top/gtidectbym.html

[S09] C：结构体定义与初始化
来源：http://hz.iojbl.cn/gtrcvhzkpv.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.aibaodan.cn/gtbpvaarud.html

[S10] C：指针与解引用
来源：http://hz.xziqi.cn/gtqggmggdm.html

int *p = &a;  *p = 5;
来源：http://hz.zhengqikj.top/gtrfjwgvep.html

[S11] C：逐行读文件
来源：http://hz.xuetiantiany.cn/gtofzaqaab.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.yongpay.top/gtsrftsdsi.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.zhijiandao.cn/gtkfjnnxjl.html

fclose(f);
来源：http://hz.jinyuanbaomall.cn/gtuobwmkdn.html

[S12] C：写文件
来源：http://hz.shuidangran.top/gttphbiuyj.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.daxiang520.top/gtbbqsvdsl.html

[S13] C：宏定义
来源：http://hz.tianlin.xyz/gtmigqfgbo.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.guannengcc.top/gtvfiijswj.html

[S14] C：枚举
来源：http://hz.birdmap.top/gtstiituek.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.shzxlz.cn/gteuprgegi.html

[S15] C：类型转换
来源：http://hz.yj20258.top/gtjgkrcitn.html

(double) a / b
来源：http://hz.yuxming.cn/gtgcldmpxz.html

[S16] C：位操作置位
来源：http://hz.tanke756.top/gthfqecdhm.html

x |= (1 << 3);
来源：http://hz.haohaochexian.top/gtxjdyphgy.html

[S17] C：安全拼接字符串
来源：http://hz.gzhubu.top/gtuqgbmgci.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.birdmap.top/gtzcjemhpv.html

[S18] C：命令行参数
来源：http://hz.sufxvd.cn/gtvigdbqka.html

int main(int argc, char **argv)
来源：http://hz.bjfxy.top/gtwizxvcvl.html

[S19] C：快速排序
来源：http://hz.chenjidiqi.icu/gtnivutckt.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.shzxlz.cn/gtmjvdokat.html

[S20] C：二分查找
来源：http://hz.xinyue.icu/gtbpqufevd.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.hongshengwenyu.top/gtxoewwfho.html

[S21] C：字符类别判断
来源：http://hz.sweek.top/gtujdcohlb.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.chenjidiqi.icu/gtxkhtexsu.html

[S22] C：字符串转数字
来源：http://hz.hnqzz.top/gtvkalryoi.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.0kj1m.cn/gtzrlbjskv.html

[S23] C：随机数
来源：http://hz.iojbl.cn/gtgxzielqz.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.daxiang520.top/gtrncjltlz.html

[S24] C：获取本地时间
来源：http://hz.fengsongda.top/gtvqwclsvy.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.shanyushiyangkeji.top/gtvffkhvxr.html

[S25] C：内存拷贝
来源：http://hz.xinyue.icu/gtedadrlog.html

memcpy(dst, src, n);
来源：http://hz.hfpthk.cn/gtdiljiwne.html

[S26] C：内存清零
来源：http://hz.redwolf501.top/gtkzpuoylo.html


<!-- 参考信息 -->