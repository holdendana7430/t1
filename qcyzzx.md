代发 wailian999

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.gzhubu.top/gttxarehxg.html

[Q58] 累计求和
来源：http://hz.nwbrower.top/gtlifdivqj.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.jiagoushi.top/gtwfhokxts.html

[Q59] 分组内累计
来源：http://hz.chenlongwang.top/gtldfaigqe.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.sufxvd.cn/gtbwnjxxws.html

[Q60] 取上一行 / 下一行
来源：http://hz.gzhubu.top/gtbntqaqxq.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.jinghuilouyu.cn/gtrjqpwhdd.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.yueranfly.top/gttkjacddm.html

[Q61] 移动平均
来源：http://hz.hnxiangtu.top/gtcwndsjlm.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.havefunace.top/gtzxlpvyhf.html

[Q62] 分组占比
来源：http://hz.316326.xyz/gtwxwxkiye.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.svipenyu.cn/gtbmvvcyng.html

[Q63] 开启事务
来源：http://hz.0kj1m.cn/gtdkhqajcf.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.smart0.xyz/gtddevtkrh.html

[Q64] 提交事务
来源：http://hz.zhengqikj.top/gtetesjjtt.html

COMMIT;
来源：http://hz.guowangkeji.top/gtrugtrezy.html

[Q65] 回滚事务
来源：http://hz.kuanghao11.cn/gtmncswwbj.html

ROLLBACK;
来源：http://hz.quarkkingdee.top/gtabgnlmzg.html

[Q66] 行锁查询
来源：http://hz.shuidangran.top/gtaqoaarrj.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.sweek.top/gtdvolhdgu.html

[Q67] 设置隔离级别
来源：http://hz.aibaodan.cn/gthvlctsuc.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.zdqjudy.top/gtochfnrfg.html

[Q68] 保存点
来源：http://hz.ywan-chungtsiang.top/gtbqulbvwl.html

SAVEPOINT sp1;
来源：http://hz.jinqigfzy.top/gtaoqtqjoz.html

ROLLBACK TO sp1;
来源：http://hz.jinqigufen.top/gtdqqdxyrl.html

[Q69] 查看执行计划
来源：http://hz.hnxiangtu.top/gtwecmbwnf.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.ywan-chungtsiang.top/gtdatahrxe.html

[Q70] 更新统计信息
来源：http://hz.wangshuangyany.cn/gtwbcbzvhe.html

ANALYZE TABLE users;
来源：http://hz.dashuyun.cn/gtovbpvihl.html

[Q71] 查看建表语句
来源：http://hz.nanxuanxn.top/gtraknyujv.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.wangshuangyany.cn/gtpawelnat.html

[Q72] 查看索引
来源：http://hz.vqdsnc.cn/gtzsafgmzz.html

SHOW INDEX FROM users;
来源：http://hz.ydzc1.top/gtantlikdy.html

[Q73] 查看表状态
来源：http://hz.hongshengwenyu.top/gtzygkrfpj.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.mhx1999.top/gtldctaekr.html

[Q74] 强制使用索引
来源：http://hz.ydzc1.top/gtrzvgjmpe.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.jinghuilouyu.cn/gtjparbmso.html

[Q75] 日期格式化
来源：http://hz.jianghu66.top/gtlcaynytc.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.bjfxy.top/gtozlgyvsl.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.yueranfly.top/gtdoizfpve.html

[Q76] 按天统计
来源：http://hz.guannengcc.top/gtniviaehs.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.jinyuanbaomall.cn/gttsrjxaup.html

[Q77] 时间加减
来源：http://hz.cqqwz.cn/gthzbyjxgw.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.sxryk.cn/gtamttoajt.html

[Q78] 当前时间
来源：http://hz.jqgufenzy.top/gtgjuqlbec.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.aibaodan.cn/gtjuvusoax.html

[Q79] 字符串拼接
来源：http://hz.zhongyouzk.top/gtajwuxull.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.fengsongda.top/gtmktahggp.html

[Q80] 字符串截取
来源：http://hz.jinqigfzy.top/gtdxjjkjje.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.gzhubu.top/gtasmhhczd.html

[Q81] 字符串替换
来源：http://hz.jqgufenzy.top/gtorjstrwm.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.shzxlz.cn/gtkydrbhtx.html

[Q82] 字符长度与字节长度
来源：http://hz.hammf.cn/gtsuorblnu.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.shangyingyoupin.top/gtuoslcxoi.html

[Q83] 大小写转换
来源：http://hz.yangfankeji.com/gtdzlhyggl.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.shuidangran.top/gtutiqdvlg.html

[Q84] 去除首尾空格
来源：http://hz.kuanghao11.cn/gtcfppjgfp.html

SELECT TRIM(name) FROM users;
来源：http://hz.aizwys.cn/gtngzmuljd.html

[Q85] 数值取整
来源：http://hz.fengsongda.top/gtvfhbeyrb.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.pengpengdd.cyou/gtgfbyxiqd.html

[Q86] 读取 JSON 字段
来源：http://hz.dashuyun.cn/gtrmdttlpx.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.jinghuilouyu.cn/gtyaivyxaa.html

[Q87] JSON 字段做条件
来源：http://hz.kuanghao11.cn/gtktunpptk.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.ydzc1.top/gtpgcfrdmb.html

[Q88] 行转列（条件聚合）
来源：http://hz.hfpthk.cn/gtmdzuxuxz.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.jinyuanbaomall.cn/gtvwukaqqt.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.52xcode.cn/gtwgyszyjz.html

[Q89] 判断表是否存在
来源：http://hz.dashuyun.cn/gttzblvskg.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.ydjk.org.cn/gtbzquodmf.html

[Q90] 生成序号列
来源：http://hz.nanxinkj.top/gtuddahvvg.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.yvedp.cn/gtfpcyqqra.html

================================================================================
来源：http://hz.kuanghao11.cn/gtdsbksulp.html

R. Bash 专题
来源：http://hz.andypj.xyz/gtdcnqqqxj.html

================================================================================
来源：http://hz.zhixingplan.top/gtctigmdky.html

[R01] shebang 与严格模式
来源：http://hz.jlsjyb.cn/gtqplxoceb.html

#!/usr/bin/env bash
来源：http://hz.xinyue.icu/gtimlwpxvx.html

set -euo pipefail
来源：http://hz.zhijiandao.cn/gthbeobgfg.html

[R02] 变量赋值与使用
来源：http://hz.quarkkingdee.top/gtqgkncvle.html

name="Tom"; echo "$name"
来源：http://hz.cqqwz.cn/gtnmxpejly.html

[R03] 只读变量
来源：http://hz.gogol.net.cn/gtdrtadvdi.html

readonly PI=3.14
来源：http://hz.ydzc1.top/gtpsknmgnj.html

[R04] 位置参数
来源：http://hz.jqgfzy.top/gtdtyeanlp.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.yueranfly.top/gtbimdtvhf.html

[R05] 参数默认值
来源：http://hz.xylfe.cn/gtzuxcqtfr.html

name="${1:-default}"
来源：http://hz.gogol.net.cn/gtdehejibf.html

[R06] 判断命令是否存在
来源：http://hz.yonumen.top/gtgckqfcwl.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.zhixingplan.top/gtmcwaeqpe.html

[R07] if 判断文件
来源：http://hz.aizwys.cn/gtqccauspw.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.sweek.top/gtqflguvwl.html

[R08] 数值比较
来源：http://hz.shanyushiyangtech.top/gtvvlnfliw.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.iojbl.cn/gtdtbtxdjm.html

[R09] 字符串比较
来源：http://hz.yj202588.top/gtwxxxzmlj.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.feifeiyinyue.top/gtobriyxtx.html

[R10] 正则匹配
来源：http://hz.jinqigfzy.top/gtddfytgwo.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.9152youxi.cn/gtlanlhqjs.html

[R11] case 多分支
来源：http://hz.smart0.xyz/gtjcogrbju.html

case "$1" in
来源：http://hz.tanke756.top/gtmfojwoxg.html

start) echo "启动" ;;
来源：http://hz.jinqigufen.top/gthjbqaayz.html

stop)  echo "停止" ;;
来源：http://hz.jinqigfzy.top/gtwrprrvcb.html

*)     echo "未知命令" ;;
来源：http://hz.aizwys.cn/gthunnwaun.html

esac
来源：http://hz.zhijiandao.cn/gtkipvmnag.html

[R12] for 遍历文件
来源：http://hz.jqgufenzy.top/gtcxhqrfso.html

for f in *.txt; do echo "$f"; done
来源：http://hz.316326.xyz/gtungkklsl.html

[R13] for 计数循环
来源：http://hz.feifeiyinyue.top/gtkjceolby.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.feifeiyinyue.top/gtttmxmxxg.html

[R14] C 风格 for
来源：http://hz.jiagoushi.top/gtmshuricm.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.zhixingplan.top/gtohcmeljp.html

[R15] while 逐行读文件
来源：http://hz.haohaochexian.top/gtqsdhzymo.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.cdnleiting.top/gtiamzemfy.html

[R16] until 等待条件
来源：http://hz.shuidangran.top/gtclxujsnh.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.kuanghao11.cn/gtfelkqeqd.html

[R17] 数组定义与取值
来源：http://hz.316326.xyz/gtlavodhta.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.jinghuilouyu.cn/gtgmnpowoj.html

[R18] 遍历数组
来源：http://hz.shanyushiyangtech.top/gtoskzemen.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.yangfankeji.com/gttfkuknuf.html

[R19] 数组长度
来源：http://hz.cheryme.top/gtzkyhqpbn.html

echo "${#arr[@]}"
来源：http://hz.guowangkeji.top/gttyofdpkt.html

[R20] 关联数组（字典）
来源：http://hz.iojbl.cn/gtpirmzkxx.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.cheryme.top/gtgesqzmyf.html

[R21] 字符串长度
来源：http://hz.shanyushiyangtech.top/gtrqmbxytk.html

echo "${#s}"
来源：http://hz.pengpengdd.cyou/gtpzehlzdi.html

[R22] 截取子串
来源：http://hz.aizwys.cn/gtctvakppb.html

echo "${s:0:5}"
来源：http://hz.zhijiandao.cn/gtmarhcucf.html

[R23] 字符串替换
来源：http://hz.nwbrower.top/gtaexkyjej.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.xziqi.cn/gtrbpylbfs.html

[R24] 大小写转换
来源：http://hz.jqgufenzy.top/gtpowabpps.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.shanyushiyangtech.top/gthrsbzwum.html

[R25] 去后缀 / 去前缀
来源：http://hz.pengpengdd.cyou/gtyfsdisis.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.yueranfly.top/gtfmuqzmuw.html

[R26] 命令替换
来源：http://hz.nanxuanxn.top/gtkcvdnluh.html

now=$(date +%F); echo "$now"
来源：http://hz.yj20258.top/gtinkzojoc.html

[R27] 算术展开
来源：http://hz.wangshuangyany.cn/gtccxasbrs.html

echo $((1 + 2 * 3))
来源：http://hz.snrcjt.cn/gtqprcfpqj.html

[R28] 浮点运算
来源：http://hz.zhaomingkeji.xyz/gtamymksnk.html

echo "scale=2; 10/3" | bc
来源：http://hz.9152youxi.cn/gtynsdsgwi.html

[R29] 定义函数
来源：http://hz.meibo888.top/gtaonhsshu.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.ivvv.top/gtzlfoysyu.html

[R30] 函数返回状态码
来源：http://hz.jinghuilouyu.cn/gtfworrerx.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.zhijiandao.cn/gtfkdrbbhj.html

[R31] 局部变量
来源：http://hz.ehwqpu.com/gtcvewzfbi.html

f() { local x=1; echo "$x"; }
来源：http://hz.yj202588.top/gtnbqncxqs.html

[R32] 参数个数校验
来源：http://hz.birdmap.top/gtridfueqb.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.dianchejie.cn/gtpnzjyvdm.html

[R33] 捕获错误并提示行号
来源：http://hz.yuxming.cn/gtyeutwecn.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.xuanzx.com/gtqeptkqnu.html

[R34] 退出时清理
来源：http://hz.jianghu66.top/gtbwupwafl.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.tanke756.top/gthtgfwnte.html

[R35] 后台执行并等待
来源：http://hz.shanyushiyangtech.top/gtafydwssw.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.zhiwuduotai.top/gtbvbvhdel.html

[R36] 并发执行多个任务
来源：http://hz.yangfankeji.com/gtfvdfuuui.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.nanxuanxn.top/gtgsdctcxm.html

[R37] 把输出赋给变量
来源：http://hz.yonumen.top/gtwdmhxrsl.html

files=$(ls -1)
来源：http://hz.zhiwuduotai.top/gtizjxoyrq.html

[R38] 管道串联
来源：http://hz.quarkkingdee.top/gtlhhxgkem.html

cat a.txt | grep -i error | wc -l
来源：http://hz.tian-w.cn/gtushhoeah.html

[R39] 重定向标准输出与错误
来源：http://hz.tian-w.cn/gttajpbidv.html

cmd > out.log 2>&1
来源：http://hz.jinqigufen.top/gtvfwgqaoe.html

[R40] 追加写日志
来源：http://hz.yongpay.top/gtgthxeyzs.html

echo "log" >> out.log
来源：http://hz.zhixingplan.top/gtzsuqokum.html

[R41] 丢弃输出
来源：http://hz.zhixingplan.top/gtrkgfldok.html

cmd >/dev/null 2>&1
来源：http://hz.sufxvd.cn/gteudusbjv.html

[R42] 输入重定向
来源：http://hz.shanyushiyangtech.top/gtedzmbqgn.html

wc -l < a.txt
来源：http://hz.aibaodan.cn/gtdjpnelan.html

[R43] 按名字查找文件
来源：http://hz.316326.xyz/gtzwsqqokq.html

find . -name "*.log" -type f
来源：http://hz.gogol.net.cn/gtgemmzsqf.html

[R44] 按修改时间查找
来源：http://hz.sweek.top/gtjtybzqkb.html

find . -mtime -7 -type f
来源：http://hz.gzhubu.top/gtxgxcjucq.html

[R45] 批量删除
来源：http://hz.shangyingyoupin.top/gtjnyiyljp.html

find . -name "*.tmp" -delete
来源：http://hz.cqqwz.cn/gtsbsxleqa.html

[R46] 递归替换文件内容
来源：http://hz.hammf.cn/gtgidsdgyl.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.jinghuilouyu.cn/gtjlxwgtot.html

[R47] sed 单行替换
来源：http://hz.yj20258.top/gtvtjfuiyd.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.xylfe.cn/gtlfcxxcfa.html

[R48] awk 取指定列
来源：http://hz.jyoumei.cn/gtiexqkptk.html

awk '{print $1, $3}' a.txt
来源：http://hz.yj202588.top/gtjbqbltcp.html

[R49] awk 带条件
来源：http://hz.hywenlv.cn/gtptatvmnm.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.zycfv.cn/gtuushqvnq.html

[R50] awk 求和
来源：http://hz.snrcjt.cn/gtescnjdqj.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.hongshengwenyu.top/gtvwevsypc.html

[R51] 排序去重取前几
来源：http://hz.guowangkeji.top/gtozyfpsoi.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.xingfuxueyuan.xyz/gtjffkktqh.html

[R52] 统计行数
来源：http://hz.nanxuanxn.top/gtndtqnfvl.html

wc -l a.txt
来源：http://hz.yonumen.top/gtyntfvmev.html

[R53] 查看文件头与实时尾
来源：http://hz.haohaochexian.top/gtomeafsqj.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.yanxiufei.cn/gtimsuwqkx.html

[R54] 比较两个文件
来源：http://hz.hammf.cn/gtluczenbj.html

diff a.txt b.txt
来源：http://hz.yj202588.top/gtzkjvsbnu.html

[R55] 压缩与解压
来源：http://hz.snrcjt.cn/gtopwesgfc.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.hnxiangtu.top/gtfpmysxmy.html

[R56] 远程拷贝
来源：http://hz.meibo888.top/gtiqutsexh.html

scp file user@host:/path/
来源：http://hz.quarkkingdee.top/gtasjvtwjx.html

[R57] 远程执行命令
来源：http://hz.jlsjyb.cn/gtwiqjypld.html

ssh user@host 'uptime'
来源：http://hz.zhijiandao.cn/gtzqcqzcup.html

[R58] 下载文件
来源：http://hz.zhaomingkeji.xyz/gtmpaocstw.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.jqgfzy.top/gtaifuwxxb.html

[R59] 发 POST JSON
来源：http://hz.aibaodan.cn/gtpyggijte.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.zhoulong.xyz/gtyxgscddq.html

[R60] 只看 HTTP 状态码
来源：http://hz.cashguo.top/gtmkxovcqo.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.jianghu66.top/gtkgpsyleu.html

[R61] 磁盘占用
来源：http://hz.fzhhl.top/gtytrcauyq.html

df -h;  du -sh *
来源：http://hz.ydzc1.top/gttuoribkw.html

[R62] 找最占空间的文件
来源：http://hz.tianlin.xyz/gttvdnwyax.html

du -ah . | sort -rh | head -10
来源：http://hz.sufxvd.cn/gtmuggnxam.html

[R63] 内存与进程
来源：http://hz.jinyuanbaomall.cn/gtlkdjcqjp.html

free -h;  ps aux | grep nginx
来源：http://hz.hnxiangtu.top/gthnavfhtn.html

[R64] 结束进程
来源：http://hz.chenjidiqi.icu/gtukvztepl.html

kill -9 $(pgrep -f app.py)
来源：http://hz.hnxiangtu.top/gtwrziwosn.html

[R65] 查看端口占用
来源：http://hz.pycfn.com/gtmeaklpkm.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.mhx1999.top/gtwthxpmhi.html

[R66] 定时任务
来源：http://hz.sysykeji.top/gtkmlsznyb.html

crontab -e;  crontab -l
来源：http://hz.pycfn.com/gtmhcjqpqj.html

[R67] 生成随机十六进制串
来源：http://hz.cqqwz.cn/gtfufemrng.html

openssl rand -hex 16
来源：http://hz.wangdashe.top/gtsiwcmire.html

[R68] 计算文件校验值
来源：http://hz.0kj1m.cn/gtyspcwelc.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.zhoulong.xyz/gtnuunuclm.html

[R69] 生成随机密码
来源：http://hz.cashguo.top/gtusohybrf.html

head -c 16 /dev/urandom | base64
来源：http://hz.hysaishi.cn/gtapevevac.html

[R70] 时间戳与互转
来源：http://hz.haohaochexian.top/gtcaphzejn.html

date +%s;  date -d @1700000000
来源：http://hz.jianghu66.top/gthbhbuitl.html

[R71] 日期格式化
来源：http://hz.ybcxt.top/gtcywghxbf.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.jinqigfzy.top/gthctkfpmg.html

[R72] 等待端口就绪
来源：http://hz.sweek.top/gtyoijobwq.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.fzhhl.top/gtzcrglwux.html

[R73] 分割大日志
来源：http://hz.yj20258888.top/gttqolazxx.html

split -l 1000 big.log part_
来源：http://hz.nanxinkj.top/gtvsvtncbb.html

[R74] 批量重命名
来源：http://hz.andypj.xyz/gtsyitdzyb.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.hongshengwenyu.top/gtaftcpoor.html

[R75] 导出环境变量
来源：http://hz.cashguo.top/gtuapwygce.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.52xcode.cn/gtbrrvtidu.html

[R76] 使用临时文件
来源：http://hz.xylfe.cn/gtkvxtltst.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.wangshuangyany.cn/gtqkkqsfqo.html

[R77] 读取用户输入
来源：http://hz.c1oappe.top/gtrljwpfwr.html

read -rp "请输入: " ans
来源：http://hz.shangyingyoupin.top/gtfcmsqmuh.html

[R78] 交互式菜单
来源：http://hz.zhoulong.xyz/gtwhxqqtgz.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.316326.xyz/gtbuelshjp.html

[R79] 解析命令行选项
来源：http://hz.sxryk.cn/gtybzuxkaa.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.mhx1999.top/gtayzkeplu.html

[R80] 查看脚本执行耗时
来源：http://hz.svipenyu.cn/gtetblrncr.html

time ./run.sh
来源：http://hz.yanxiufei.cn/gtigqwwyio.html

================================================================================
来源：http://hz.hnxiangtu.top/gtbksbagnk.html

S. C / C++ 专题
来源：http://hz.zhixingplan.top/gtcoayodyk.html

================================================================================
来源：http://hz.fengsongda.top/gtvbzfdiya.html

[S01] C：Hello World
来源：http://hz.jinqigufen.top/gtasaragki.html

#include <stdio.h>
来源：http://hz.yonumen.top/gtlitjtlfl.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.hnxiangtu.top/gtmziblzrv.html

[S02] C：变量与格式化输出
来源：http://hz.hnqzz.top/gtgmcwzmow.html

int a = 10; printf("%d\n", a);
来源：http://hz.hongshengwenyu.top/gtjbfflbsg.html

[S03] C：读入整数
来源：http://hz.snrcjt.cn/gttqrzdufk.html

int x; scanf("%d", &x);
来源：http://hz.hongshengwenyu.top/gteknrhsxb.html

[S04] C：字符串复制
来源：http://hz.yj20258888.top/gtjnqkjohg.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.zhongyouzk.top/gtbzqistgv.html

[S05] C：字符串长度
来源：http://hz.gzhubu.top/gtzkjsgsdb.html

strlen(s)
来源：http://hz.yonumen.top/gtnabxzbxh.html

[S06] C：字符串比较
来源：http://hz.jqgufenzy.top/gtxqnmjbfw.html

strcmp(a, b) == 0
来源：http://hz.dianchejie.cn/gtgmorjaul.html

[S07] C：数组遍历求和
来源：http://hz.yvedp.cn/gtbfhqdgdq.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.aibaodan.cn/gtngqfqogs.html

[S08] C：动态内存分配与释放
来源：http://hz.birdmap.top/gtdevsgsmf.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.shanyushiyangkeji.top/gtdjfqjuzt.html

[S09] C：结构体定义与初始化
来源：http://hz.dashuyun.cn/gtjyyljehy.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.yueranfly.top/gttddxuldg.html

[S10] C：指针与解引用
来源：http://hz.redwolf501.top/gtnnvzrics.html

int *p = &a;  *p = 5;
来源：http://hz.cdnleiting.top/gthxidqajq.html

[S11] C：逐行读文件
来源：http://hz.kuanghao11.cn/gthbfveroi.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.quarkkingdee.top/gtymclqwam.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.dashuyun.cn/gtjtocpffd.html

fclose(f);
来源：http://hz.iojbl.cn/gtvpetpesi.html

[S12] C：写文件
来源：http://hz.yj20258888.top/gtaoxejahu.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.jlsjyb.cn/gtnmxphjci.html

[S13] C：宏定义
来源：http://hz.ydjk.org.cn/gtstwptilv.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.nwbrower.top/gtrzxoknxu.html

[S14] C：枚举
来源：http://hz.jinqigufen.top/gtoczjftvr.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.nanxinkj.top/gtfabwnftl.html

[S15] C：类型转换
来源：http://hz.jinqigufen.top/gtylfutpvb.html

(double) a / b
来源：http://hz.nanxuanxn.top/gtmbpsaacn.html

[S16] C：位操作置位
来源：http://hz.hnxiangtu.top/gtwlrftceg.html

x |= (1 << 3);
来源：http://hz.haohaochexian.top/gtmevlwzet.html

[S17] C：安全拼接字符串
来源：http://hz.yj20258888.top/gtbzghxorm.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.redwolf501.top/gteeuihyna.html

[S18] C：命令行参数
来源：http://hz.jinqigfzy.top/gtyrspyvup.html

int main(int argc, char **argv)
来源：http://hz.316326.xyz/gtbkdwpmpx.html

[S19] C：快速排序
来源：http://hz.nanxuanxn.top/gtreeceyyr.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.ydjk.org.cn/gtabjyrqee.html

[S20] C：二分查找
来源：http://hz.birdmap.top/gtuyjjvoxz.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.0kj1m.cn/gtvrkqyqnq.html

[S21] C：字符类别判断
来源：http://hz.jinqigfzy.top/gtvokmzxbz.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.hongshengwenyu.top/gtorwddjjj.html

[S22] C：字符串转数字
来源：http://hz.xziqi.cn/gtodzpulyd.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.tanke756.top/gtkqynndgn.html

[S23] C：随机数
来源：http://hz.birdmap.top/gtlvmnbjnq.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.gogol.net.cn/gtrgyjxivz.html

[S24] C：获取本地时间
来源：http://hz.chenlongwang.top/gtbbxtvlcq.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.xingfuxueyuan.xyz/gtwkzbmfue.html

[S25] C：内存拷贝
来源：http://hz.pycfn.com/gtzrwktewp.html

memcpy(dst, src, n);
来源：http://hz.zhijiandao.cn/gtabyzciof.html

[S26] C：内存清零
来源：http://hz.ppjwa.cn/gtbidqriru.html

memset(a, 0, sizeof a);
来源：http://hz.daxiang520.top/gtipkqrtlx.html

[S27] C：定义常量
来源：http://hz.gogol.net.cn/gtnjbfthxq.html

const double PI = 3.14159;
来源：http://hz.0kj1m.cn/gthvanvapp.html

[S28] C：静态变量
来源：http://hz.yvedp.cn/gtqgndbmqo.html


<!-- 参考信息 -->