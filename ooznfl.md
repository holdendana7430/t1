代发 wailian999

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.pengpengdd.cyou/gtmqlhwgot.html

[Q54] 清空表
来源：http://hz.hfpthk.cn/gtrlqcxnnk.html

TRUNCATE TABLE logs;
来源：http://hz.guannengcc.top/gtfhjkzdln.html

[Q55] 排名（并列占位）
来源：http://hz.jyoumei.cn/gtsxojdhts.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.ybcxt.top/gtlzkjyhxq.html

[Q56] 密集排名（并列不占位）
来源：http://hz.yj20258888.top/gtfszukduj.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.ydjk.org.cn/gtuzuudkpz.html

[Q57] 行号
来源：http://hz.pengpengdd.cyou/gtmexlkxml.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.guannengcc.top/gtabxmnamk.html

[Q58] 累计求和
来源：http://hz.haohaochexian.top/gtmuvlpewz.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.sxryk.cn/gtwcruzfaz.html

[Q59] 分组内累计
来源：http://hz.cheryme.top/gtyjyxbrpk.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.yangfankeji.com/gtkafwtijs.html

[Q60] 取上一行 / 下一行
来源：http://hz.zdqjudy.top/gttlciahgr.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.feifeiyinyue.top/gtzceifata.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.dianchejie.cn/gttwgcoicj.html

[Q61] 移动平均
来源：http://hz.jqgfzy.top/gttjagnpbe.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.sufxvd.cn/gtxtiinqdi.html

[Q62] 分组占比
来源：http://hz.birdmap.top/gtuxbcfkkj.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.shanyushiyangtech.top/gtdeiaaazq.html

[Q63] 开启事务
来源：http://hz.zycfv.cn/gtcouirbag.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.nanxuanxn.top/gtzvrysjll.html

[Q64] 提交事务
来源：http://hz.ydzc1.top/gtuqdeixmn.html

COMMIT;
来源：http://hz.jinyuanbaomall.cn/gtgzzcqqce.html

[Q65] 回滚事务
来源：http://hz.aizwys.cn/gtfvvjujnc.html

ROLLBACK;
来源：http://hz.havefunace.top/gtiebrwuld.html

[Q66] 行锁查询
来源：http://hz.jinghuilouyu.cn/gtijxydmiw.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.yj202588.top/gtofdbhago.html

[Q67] 设置隔离级别
来源：http://hz.zhixingplan.top/gtoiisigsb.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.fzhhl.top/gtebcwawhw.html

[Q68] 保存点
来源：http://hz.pengpengdd.cyou/gtmlskgmde.html

SAVEPOINT sp1;
来源：http://hz.xingfuxueyuan.xyz/gtmapbmxkr.html

ROLLBACK TO sp1;
来源：http://hz.jinghuilouyu.cn/gtvsmsxaqa.html

[Q69] 查看执行计划
来源：http://hz.dianchejie.cn/gtuujbtscp.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.cucudq.cn/gtnezxoygj.html

[Q70] 更新统计信息
来源：http://hz.wangdashe.top/gtmaeictdg.html

ANALYZE TABLE users;
来源：http://hz.0kj1m.cn/gtvzshaded.html

[Q71] 查看建表语句
来源：http://hz.aizwys.cn/gttmkzhfff.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.xuanzx.com/gtfwejfyji.html

[Q72] 查看索引
来源：http://hz.nanxuanxn.top/gtnaczhdwf.html

SHOW INDEX FROM users;
来源：http://hz.feifeiyinyue.top/gtflkvmlcm.html

[Q73] 查看表状态
来源：http://hz.dashuyun.cn/gtqlxeiflq.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.9152youxi.cn/gtgeezlyom.html

[Q74] 强制使用索引
来源：http://hz.xuanzx.com/gtfqrtfywa.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.xylfe.cn/gtmtzvebtt.html

[Q75] 日期格式化
来源：http://hz.xingfuxueyuan.xyz/gtrwpbjqkc.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.hnqzz.top/gtjjopeblr.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.yj20258.top/gtiwbhxvdt.html

[Q76] 按天统计
来源：http://hz.zhijiandao.cn/gtefhzyalg.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.xingfuxueyuan.xyz/gtkkztcaud.html

[Q77] 时间加减
来源：http://hz.ybcxt.top/gtrwdixxbe.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.fengsongda.top/gtyldlfqpe.html

[Q78] 当前时间
来源：http://hz.jinghuilouyu.cn/gtaujtmeli.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.gzhubu.top/gtqxgjojqn.html

[Q79] 字符串拼接
来源：http://hz.pengpengdd.cyou/gturxrngzj.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.yj20258888.top/gturhaphjl.html

[Q80] 字符串截取
来源：http://hz.ppjwa.cn/gtvtbxjdiy.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.fzhhl.top/gtjlwgopcf.html

[Q81] 字符串替换
来源：http://hz.jqgfzy.top/gtzscowlvt.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.vqdsnc.cn/gtdnzsbtou.html

[Q82] 字符长度与字节长度
来源：http://hz.zhongyouzk.top/gtssofzstg.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.yuanzhike.top/gtbnorrkru.html

[Q83] 大小写转换
来源：http://hz.kuanghao11.cn/gtyylgrtjy.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.yj20258888.top/gtilreawtc.html

[Q84] 去除首尾空格
来源：http://hz.gzhubu.top/gtczahcstn.html

SELECT TRIM(name) FROM users;
来源：http://hz.yj20258.top/gtcjhfhcse.html

[Q85] 数值取整
来源：http://hz.feifeiyinyue.top/gtyzhbrcqa.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.gotoacloud.top/gtdmfwzsiq.html

[Q86] 读取 JSON 字段
来源：http://hz.tanke756.top/gtzzzbwbdo.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.316326.xyz/gtvmpylujy.html

[Q87] JSON 字段做条件
来源：http://hz.iojbl.cn/gtmpywjzin.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.zycfv.cn/gtxkwxaqkq.html

[Q88] 行转列（条件聚合）
来源：http://hz.yanxiufei.cn/gtqbcsdyfx.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.jinqigufen.top/gtknmgfzfs.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.sysykeji.top/gtkufswoul.html

[Q89] 判断表是否存在
来源：http://hz.9152youxi.cn/gtwtuafhkt.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.tanke756.top/gthzuwppfx.html

[Q90] 生成序号列
来源：http://hz.pengpengdd.cyou/gtjzssgibn.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.sweek.top/gtykechysp.html

================================================================================
来源：http://hz.hnxiangtu.top/gtuyremhqv.html

R. Bash 专题
来源：http://hz.cucudq.cn/gtjclzzaga.html

================================================================================
来源：http://hz.zdqjudy.top/gtcqgcjgrt.html

[R01] shebang 与严格模式
来源：http://hz.gaohongyu789.top/gtvwkzycfo.html

#!/usr/bin/env bash
来源：http://hz.pycfn.com/gthlcygfao.html

set -euo pipefail
来源：http://hz.yuxming.cn/gtkehhbsej.html

[R02] 变量赋值与使用
来源：http://hz.cucudq.cn/gtjkrjmshz.html

name="Tom"; echo "$name"
来源：http://hz.nwbrower.top/gtavjgdnxl.html

[R03] 只读变量
来源：http://hz.pengpengdd.cyou/gtumtcsfnd.html

readonly PI=3.14
来源：http://hz.yj20258888.top/gtgmddaqlv.html

[R04] 位置参数
来源：http://hz.iojbl.cn/gtdlylhjel.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.haohaochexian.top/gturedigqb.html

[R05] 参数默认值
来源：http://hz.wangshuangyany.cn/gtlycsesdm.html

name="${1:-default}"
来源：http://hz.hnqzz.top/gtgpkqpslk.html

[R06] 判断命令是否存在
来源：http://hz.jqgfzy.top/gtkdphzvkv.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.sweek.top/gthlgmhuyl.html

[R07] if 判断文件
来源：http://hz.hammf.cn/gtadgiomuz.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.shuidangran.top/gtrlmoupxb.html

[R08] 数值比较
来源：http://hz.zhoulong.xyz/gtywecinoj.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.jiagoushi.top/gtjjwefuzd.html

[R09] 字符串比较
来源：http://hz.gzhubu.top/gtqcydflyu.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.zhengqikj.top/gtdyfgttev.html

[R10] 正则匹配
来源：http://hz.jinqigufen.top/gtyrqlbmtj.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.jqgufenzy.top/gtnadebsnr.html

[R11] case 多分支
来源：http://hz.yongpay.top/gtxbfkmrlq.html

case "$1" in
来源：http://hz.nwbrower.top/gtgzcyhnav.html

start) echo "启动" ;;
来源：http://hz.gaohongyu789.top/gtjfrseruv.html

stop)  echo "停止" ;;
来源：http://hz.xziqi.cn/gtofakhtbb.html

*)     echo "未知命令" ;;
来源：http://hz.chenlongwang.top/gtckogkirt.html

esac
来源：http://hz.jqgufenzy.top/gthayjuoox.html

[R12] for 遍历文件
来源：http://hz.shanyushiyangtech.top/gthnvbsvyq.html

for f in *.txt; do echo "$f"; done
来源：http://hz.bjfxy.top/gtkfelayyw.html

[R13] for 计数循环
来源：http://hz.hysaishi.cn/gtvxymdkkx.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.jinqigfzy.top/gtgacubzna.html

[R14] C 风格 for
来源：http://hz.shzxlz.cn/gtqbggvugc.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.meibo888.top/gtgezjafaw.html

[R15] while 逐行读文件
来源：http://hz.ppjwa.cn/gtpbdjwazb.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.yangfankeji.com/gttzchlbkz.html

[R16] until 等待条件
来源：http://hz.smart0.xyz/gtxjaahbfm.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.fengsongda.top/gtwpdzyrmk.html

[R17] 数组定义与取值
来源：http://hz.vqdsnc.cn/gtespajtrk.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.shuidangran.top/gtvfruliwe.html

[R18] 遍历数组
来源：http://hz.meibo888.top/gtugibcuoh.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.yj20258.top/gtbcgfvxdo.html

[R19] 数组长度
来源：http://hz.yuxming.cn/gtobuujziu.html

echo "${#arr[@]}"
来源：http://hz.tian-w.cn/gtwianehah.html

[R20] 关联数组（字典）
来源：http://hz.cqqwz.cn/gtwivhvucd.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.cashguo.top/gtqcpmzqpw.html

[R21] 字符串长度
来源：http://hz.gzhubu.top/gthinuniwb.html

echo "${#s}"
来源：http://hz.kuanghao11.cn/gtqwvdihzn.html

[R22] 截取子串
来源：http://hz.pengpengdd.cyou/gtfdhiceor.html

echo "${s:0:5}"
来源：http://hz.zhoulong.xyz/gtqarygosq.html

[R23] 字符串替换
来源：http://hz.ydzc1.top/gtfqjdhdmy.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.52xcode.cn/gteqptrjtv.html

[R24] 大小写转换
来源：http://hz.xuetiantiany.cn/gthbuvqzdd.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.chenjidiqi.icu/gtxtcarpen.html

[R25] 去后缀 / 去前缀
来源：http://hz.dianchejie.cn/gtfkzgxorg.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.jqgufenzy.top/gtuumlwhjy.html

[R26] 命令替换
来源：http://hz.gzhubu.top/gtextaxrmr.html

now=$(date +%F); echo "$now"
来源：http://hz.hnxiangtu.top/gtndembyik.html

[R27] 算术展开
来源：http://hz.hnqzz.top/gtfhgkclta.html

echo $((1 + 2 * 3))
来源：http://hz.fengsongda.top/gtcaawjgzz.html

[R28] 浮点运算
来源：http://hz.ywan-chungtsiang.top/gtdhsdutbo.html

echo "scale=2; 10/3" | bc
来源：http://hz.gaohongyu789.top/gtngncznys.html

[R29] 定义函数
来源：http://hz.shanyushiyangkeji.top/gttqkhfrdg.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.sysykeji.top/gtnxqbiqjp.html

[R30] 函数返回状态码
来源：http://hz.ivvv.top/gtrlfqcxjh.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.wangshuangyany.cn/gtddddambt.html

[R31] 局部变量
来源：http://hz.nanxinkj.top/gtjhsskiol.html

f() { local x=1; echo "$x"; }
来源：http://hz.cashguo.top/gtyzdntfgx.html

[R32] 参数个数校验
来源：http://hz.zdqjudy.top/gtobloaqgk.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.jqgufenzy.top/gtanvqthwg.html

[R33] 捕获错误并提示行号
来源：http://hz.nwbrower.top/gtdsqwpmhh.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.nwbrower.top/gtzqywwaif.html

[R34] 退出时清理
来源：http://hz.yangfankeji.com/gtqerlqqrq.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.jinqigufen.top/gttkpfjdpw.html

[R35] 后台执行并等待
来源：http://hz.tianlin.xyz/gtomgmwkbz.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.feifeiyinyue.top/gticsualiw.html

[R36] 并发执行多个任务
来源：http://hz.pycfn.com/gtlowkcmlj.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.xylfe.cn/gtfihndcfa.html

[R37] 把输出赋给变量
来源：http://hz.wangshuangyany.cn/gtpcslcgtz.html

files=$(ls -1)
来源：http://hz.yueranfly.top/gtppwfrtxr.html

[R38] 管道串联
来源：http://hz.xuanzx.com/gtcmqcodbs.html

cat a.txt | grep -i error | wc -l
来源：http://hz.gogol.net.cn/gtfzvjkvmj.html

[R39] 重定向标准输出与错误
来源：http://hz.pycfn.com/gtksdlkhel.html

cmd > out.log 2>&1
来源：http://hz.birdmap.top/gtycgoeqka.html

[R40] 追加写日志
来源：http://hz.zhixingplan.top/gtfreoxmky.html

echo "log" >> out.log
来源：http://hz.birdmap.top/gtygucmvqn.html

[R41] 丢弃输出
来源：http://hz.cucudq.cn/gtszudnrdn.html

cmd >/dev/null 2>&1
来源：http://hz.daria6918.cn/gtffjfpbxt.html

[R42] 输入重定向
来源：http://hz.guowangkeji.top/gtzkqzqxau.html

wc -l < a.txt
来源：http://hz.smart0.xyz/gtvybyymtj.html

[R43] 按名字查找文件
来源：http://hz.jinqigufen.top/gtzqwcxoxa.html

find . -name "*.log" -type f
来源：http://hz.feifeiyinyue.top/gtnetkrpps.html

[R44] 按修改时间查找
来源：http://hz.jianghu66.top/gtufssxikh.html

find . -mtime -7 -type f
来源：http://hz.dianchejie.cn/gtyudqydef.html

[R45] 批量删除
来源：http://hz.yongpay.top/gtjanvzjzy.html

find . -name "*.tmp" -delete
来源：http://hz.yonumen.top/gtqloyxgyg.html

[R46] 递归替换文件内容
来源：http://hz.bjfxy.top/gtkbrdlpng.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.redwolf501.top/gtimranans.html

[R47] sed 单行替换
来源：http://hz.jiagoushi.top/gtlgxiqlnc.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.haohaochexian.top/gtppvibyuj.html

[R48] awk 取指定列
来源：http://hz.yvedp.cn/gtgyffihmj.html

awk '{print $1, $3}' a.txt
来源：http://hz.tian-w.cn/gtvbbjmkwg.html

[R49] awk 带条件
来源：http://hz.andypj.xyz/gtusdxpguh.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.birdmap.top/gtqfnholwz.html

[R50] awk 求和
来源：http://hz.birdmap.top/gtkrregjzc.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.chenzaomai.com/gtnfgvkzwt.html

[R51] 排序去重取前几
来源：http://hz.sweek.top/gttudlbuev.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.sufxvd.cn/gthyotuswc.html

[R52] 统计行数
来源：http://hz.sysykeji.top/gtkkzgzrsx.html

wc -l a.txt
来源：http://hz.fengsongda.top/gtvncrnifr.html

[R53] 查看文件头与实时尾
来源：http://hz.hammf.cn/gtrmbceyiv.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.shanyushiyangtech.top/gtoaczcwhb.html

[R54] 比较两个文件
来源：http://hz.gzhubu.top/gtostpiigs.html

diff a.txt b.txt
来源：http://hz.andypj.xyz/gtmeztbldt.html

[R55] 压缩与解压
来源：http://hz.shuidangran.top/gtnngfifbb.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.cashguo.top/gtxuaqxtms.html

[R56] 远程拷贝
来源：http://hz.dashuyun.cn/gtlcgmtdvz.html

scp file user@host:/path/
来源：http://hz.pycfn.com/gtzkvdcksk.html

[R57] 远程执行命令
来源：http://hz.ppjwa.cn/gtgtujcnyk.html

ssh user@host 'uptime'
来源：http://hz.yanxiufei.cn/gttpockhsg.html

[R58] 下载文件
来源：http://hz.xziqi.cn/gtzgyitxzr.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.52xcode.cn/gtfctthtbq.html

[R59] 发 POST JSON
来源：http://hz.zhongyouzk.top/gtwiftyyds.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.ehwqpu.com/gtylkvmsvt.html

[R60] 只看 HTTP 状态码
来源：http://hz.mhx1999.top/gtoghvaedd.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.chenlongwang.top/gtlwodghox.html

[R61] 磁盘占用
来源：http://hz.zhijiandao.cn/gtzzidrzpc.html

df -h;  du -sh *
来源：http://hz.gogol.net.cn/gtpexblich.html

[R62] 找最占空间的文件
来源：http://hz.yonumen.top/gtknjuxzht.html

du -ah . | sort -rh | head -10
来源：http://hz.ppjwa.cn/gtoadhvfai.html

[R63] 内存与进程
来源：http://hz.tanke756.top/gtlwtavyiz.html

free -h;  ps aux | grep nginx
来源：http://hz.yongpay.top/gtqmtjjcpq.html

[R64] 结束进程
来源：http://hz.jianghu66.top/gtuokdghzl.html

kill -9 $(pgrep -f app.py)
来源：http://hz.hnqzz.top/gthxkollpf.html

[R65] 查看端口占用
来源：http://hz.xziqi.cn/gttczaqfxp.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.hnqzz.top/gtaqobxnsr.html

[R66] 定时任务
来源：http://hz.yanxiufei.cn/gthunuxwcz.html

crontab -e;  crontab -l
来源：http://hz.52xcode.cn/gtwlnjdald.html

[R67] 生成随机十六进制串
来源：http://hz.jqgufenzy.top/gtnsnzvuxv.html

openssl rand -hex 16
来源：http://hz.hnxiangtu.top/gtxgepnqgu.html

[R68] 计算文件校验值
来源：http://hz.jqgufenzy.top/gtxtlpaqaf.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.feifeiyinyue.top/gtdqyrelfs.html

[R69] 生成随机密码
来源：http://hz.iojbl.cn/gtztryofmw.html

head -c 16 /dev/urandom | base64
来源：http://hz.jinyuanbaomall.cn/gtkynmdgpn.html

[R70] 时间戳与互转
来源：http://hz.jiagoushi.top/gtytzvbdca.html

date +%s;  date -d @1700000000
来源：http://hz.zhiwuduotai.top/gtkepbekiu.html

[R71] 日期格式化
来源：http://hz.tian-w.cn/gthkonhrpo.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.hnqzz.top/gtsczxnpxh.html

[R72] 等待端口就绪
来源：http://hz.yueranfly.top/gtvlhgvoqy.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.nwbrower.top/gtqjmfxvxg.html

[R73] 分割大日志
来源：http://hz.dianchejie.cn/gtzgsrxbui.html

split -l 1000 big.log part_
来源：http://hz.birdmap.top/gtdgnldncq.html

[R74] 批量重命名
来源：http://hz.yuanzhike.top/gtvwiszsuj.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.quarkkingdee.top/gtblvfdfov.html

[R75] 导出环境变量
来源：http://hz.ivvv.top/gthdtrbdlz.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.hnxiangtu.top/gtgepuopba.html

[R76] 使用临时文件
来源：http://hz.mhx1999.top/gtucjrzijy.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.zdqjudy.top/gthgsltxkp.html

[R77] 读取用户输入
来源：http://hz.guowangkeji.top/gteuirewrx.html

read -rp "请输入: " ans
来源：http://hz.birdmap.top/gtuhhfbfhq.html

[R78] 交互式菜单
来源：http://hz.xylfe.cn/gtmslmpohu.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.316326.xyz/gtjnzobcby.html

[R79] 解析命令行选项
来源：http://hz.zhixingplan.top/gttpxadyoa.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.jiagoushi.top/gtajdozhil.html

[R80] 查看脚本执行耗时
来源：http://hz.andypj.xyz/gtsaqmfadf.html

time ./run.sh
来源：http://hz.shzxlz.cn/gtldunckms.html

================================================================================
来源：http://hz.xinyue.icu/gtfnzqdeho.html

S. C / C++ 专题
来源：http://hz.ppjwa.cn/gtsmwufugf.html

================================================================================
来源：http://hz.aizwys.cn/gtztfwofxr.html

[S01] C：Hello World
来源：http://hz.cqqwz.cn/gtbyhbbvjp.html

#include <stdio.h>
来源：http://hz.xuanzx.com/gtodgnxwkn.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.feifeiyinyue.top/gtnqbeqcbe.html

[S02] C：变量与格式化输出
来源：http://hz.0kj1m.cn/gtsqeprnov.html

int a = 10; printf("%d\n", a);
来源：http://hz.nanxinkj.top/gtvszvqgge.html

[S03] C：读入整数
来源：http://hz.pycfn.com/gtbdlyhrlu.html

int x; scanf("%d", &x);
来源：http://hz.hysaishi.cn/gtsjjymllb.html

[S04] C：字符串复制
来源：http://hz.hfpthk.cn/gtgwjyrvmo.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.smart0.xyz/gtrpiwzaby.html

[S05] C：字符串长度
来源：http://hz.shanyushiyangtech.top/gtgcihltiz.html

strlen(s)
来源：http://hz.aizwys.cn/gtoqgbvjlz.html

[S06] C：字符串比较
来源：http://hz.yvedp.cn/gtvytftlru.html

strcmp(a, b) == 0
来源：http://hz.jinqigfzy.top/gthpvijkvy.html

[S07] C：数组遍历求和
来源：http://hz.c1oappe.top/gtedvkubab.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.gotoacloud.top/gtotgziiot.html

[S08] C：动态内存分配与释放
来源：http://hz.snrcjt.cn/gtygkfaiod.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.andypj.xyz/gtpppqkjsf.html

[S09] C：结构体定义与初始化
来源：http://hz.yanxiufei.cn/gtjcaixxvt.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.shanyushiyangtech.top/gtkdyhodff.html

[S10] C：指针与解引用
来源：http://hz.gzhubu.top/gtotcqjczr.html

int *p = &a;  *p = 5;
来源：http://hz.tanke756.top/gtwopsusqo.html

[S11] C：逐行读文件
来源：http://hz.shuidangran.top/gtjjzhgzga.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.9152youxi.cn/gtxmkmeddw.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.mhx1999.top/gtmhzcjhth.html

fclose(f);
来源：http://hz.zhijiandao.cn/gtqdrbndkp.html

[S12] C：写文件
来源：http://hz.guowangkeji.top/gtkjgsraqm.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.andypj.xyz/gtyonbnzgg.html

[S13] C：宏定义
来源：http://hz.xylfe.cn/gtcsrsvkes.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.yj20258888.top/gtvfznxejr.html

[S14] C：枚举
来源：http://hz.jinghuilouyu.cn/gtxexrwxhe.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.xziqi.cn/gtpicirszi.html

[S15] C：类型转换
来源：http://hz.gaohongyu789.top/gtssgzhqbg.html

(double) a / b
来源：http://hz.mhx1999.top/gtiwkjbwbx.html

[S16] C：位操作置位
来源：http://hz.wangshuangyany.cn/gtjvyzjuuo.html

x |= (1 << 3);
来源：http://hz.tian-w.cn/gtzzkxmxlj.html

[S17] C：安全拼接字符串
来源：http://hz.quarkkingdee.top/gtsmbplupr.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.nanxinkj.top/gttuxzxpfz.html

[S18] C：命令行参数
来源：http://hz.chenlongwang.top/gtkzpopzeq.html

int main(int argc, char **argv)
来源：http://hz.bjfxy.top/gtmusegbqb.html

[S19] C：快速排序
来源：http://hz.haohaochexian.top/gtzawgfcju.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.hfpthk.cn/gttkakchhe.html

[S20] C：二分查找
来源：http://hz.ydjk.org.cn/gtsooygyvg.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.yuxming.cn/gtizuvubce.html

[S21] C：字符类别判断
来源：http://hz.sufxvd.cn/gtmwwynnaz.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.haohaochexian.top/gtpjajjxgg.html

[S22] C：字符串转数字
来源：http://hz.pengpengdd.cyou/gtkqtxbhmj.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.feifeiyinyue.top/gtqagqlwav.html

[S23] C：随机数
来源：http://hz.bjfxy.top/gtpwwqgwdz.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.yanxiufei.cn/gttpcgqxud.html

[S24] C：获取本地时间
来源：http://hz.tanke756.top/gtrdrlbsmz.html


<!-- 参考信息 -->