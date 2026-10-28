代发 wailian999

[Q65] 回滚事务
来源：http://hz.guannengcc.top/gtmzsutdhw.html

ROLLBACK;
来源：http://hz.kuanghao11.cn/gtkjcjzbyo.html

[Q66] 行锁查询
来源：http://hz.zhengqikj.top/gtyncdjsoy.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.zhijiandao.cn/gtbgocakiq.html

[Q67] 设置隔离级别
来源：http://hz.ybcxt.top/gtnwwhooxs.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.cqqwz.cn/gtttwwsape.html

[Q68] 保存点
来源：http://hz.hnxiangtu.top/gtrhtxfrbv.html

SAVEPOINT sp1;
来源：http://hz.zhoulong.xyz/gtuejffgep.html

ROLLBACK TO sp1;
来源：http://hz.fzhhl.top/gtaquahmhx.html

[Q69] 查看执行计划
来源：http://hz.aizwys.cn/gtqigsepza.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.jinyuanbaomall.cn/gttilfruqt.html

[Q70] 更新统计信息
来源：http://hz.gotoacloud.top/gtjgudpamz.html

ANALYZE TABLE users;
来源：http://hz.zhixingplan.top/gtsczjtean.html

[Q71] 查看建表语句
来源：http://hz.daxiang520.top/gtunxerifw.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.havefunace.top/gtipgxnlik.html

[Q72] 查看索引
来源：http://hz.svipenyu.cn/gtgotkwkye.html

SHOW INDEX FROM users;
来源：http://hz.dashuyun.cn/gtfvtzuqzb.html

[Q73] 查看表状态
来源：http://hz.jinqigufen.top/gtmcxwktny.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.xuanzx.com/gtfsjunfii.html

[Q74] 强制使用索引
来源：http://hz.jyoumei.cn/gttcmefvea.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.jinghuilouyu.cn/gtxqxhobwi.html

[Q75] 日期格式化
来源：http://hz.gaohongyu789.top/gtxfzxsgol.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.ybcxt.top/gtnhvrsgei.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.cucudq.cn/gtcserasro.html

[Q76] 按天统计
来源：http://hz.cheryme.top/gtgarixomi.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.shangyingyoupin.top/gtovwfmhro.html

[Q77] 时间加减
来源：http://hz.ppjwa.cn/gtawicdvad.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.sxryk.cn/gthruntvep.html

[Q78] 当前时间
来源：http://hz.c1oappe.top/gtnusphbdk.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.zhijiandao.cn/gtzzbgloqy.html

[Q79] 字符串拼接
来源：http://hz.yj20258888.top/gtyahutcuq.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.jinqigfzy.top/gtgfybqtap.html

[Q80] 字符串截取
来源：http://hz.ppjwa.cn/gtsaxlstyp.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.hongshengwenyu.top/gtbgnhupdb.html

[Q81] 字符串替换
来源：http://hz.yuxming.cn/gttczqgayr.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.snrcjt.cn/gtslrmcwmm.html

[Q82] 字符长度与字节长度
来源：http://hz.nanxinkj.top/gtqjlexsbj.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.zhaomingkeji.xyz/gtmjincldl.html

[Q83] 大小写转换
来源：http://hz.ywan-chungtsiang.top/gtujsjmwoq.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.shzxlz.cn/gtyqtvuerb.html

[Q84] 去除首尾空格
来源：http://hz.52xcode.cn/gtqecelagv.html

SELECT TRIM(name) FROM users;
来源：http://hz.guowangkeji.top/gtuhzsoikk.html

[Q85] 数值取整
来源：http://hz.shuidangran.top/gtblzqurtv.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.chenzaomai.com/gtenshrjil.html

[Q86] 读取 JSON 字段
来源：http://hz.redwolf501.top/gtuqkibdny.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.chenzaomai.com/gtaarmyaki.html

[Q87] JSON 字段做条件
来源：http://hz.zhaomingkeji.xyz/gtuhofexii.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.shzxlz.cn/gttppqdrna.html

[Q88] 行转列（条件聚合）
来源：http://hz.guannengcc.top/gthwaqqffr.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.tianlin.xyz/gtjghtxrtf.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.bjfxy.top/gtowutwdzj.html

[Q89] 判断表是否存在
来源：http://hz.guowangkeji.top/gtzqrgxcep.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.jqgfzy.top/gtmdrlehmc.html

[Q90] 生成序号列
来源：http://hz.guowangkeji.top/gterbafwgs.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.jinqigfzy.top/gtvqsiyywx.html

================================================================================
来源：http://hz.xuanzx.com/gtmtcdbohh.html

R. Bash 专题
来源：http://hz.jinghuilouyu.cn/gtfcncwnhi.html

================================================================================
来源：http://hz.yanxiufei.cn/gtbzuarchz.html

[R01] shebang 与严格模式
来源：http://hz.xingfuxueyuan.xyz/gtfxsbsxac.html

#!/usr/bin/env bash
来源：http://hz.yongpay.top/gtntxnvwql.html

set -euo pipefail
来源：http://hz.yanxiufei.cn/gtyipktksx.html

[R02] 变量赋值与使用
来源：http://hz.shanyushiyangkeji.top/gtgqokggrk.html

name="Tom"; echo "$name"
来源：http://hz.ydjk.org.cn/gtclydyaqe.html

[R03] 只读变量
来源：http://hz.shangyingyoupin.top/gthdpokyrc.html

readonly PI=3.14
来源：http://hz.guowangkeji.top/gtfgnwqsll.html

[R04] 位置参数
来源：http://hz.hongshengwenyu.top/gtfyaijdep.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.hnqzz.top/gtjrmhlbvs.html

[R05] 参数默认值
来源：http://hz.aibaodan.cn/gtxffshwrp.html

name="${1:-default}"
来源：http://hz.jlsjyb.cn/gtsqgopchq.html

[R06] 判断命令是否存在
来源：http://hz.shangyingyoupin.top/gtfnqltldj.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.pycfn.com/gtrgcksepo.html

[R07] if 判断文件
来源：http://hz.yonumen.top/gtflccaqdt.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.yvedp.cn/gtlopmkmmj.html

[R08] 数值比较
来源：http://hz.wangshuangyany.cn/gtnemggfhk.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.c1oappe.top/gtkjbjusge.html

[R09] 字符串比较
来源：http://hz.jianghu66.top/gtzfkafpgx.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.ydjk.org.cn/gtzxxrjopy.html

[R10] 正则匹配
来源：http://hz.zdqjudy.top/gtjnrdusth.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.aibaodan.cn/gtwfvuscyt.html

[R11] case 多分支
来源：http://hz.wangshuangyany.cn/gtcshiboxw.html

case "$1" in
来源：http://hz.kuanghao11.cn/gtmikovpey.html

start) echo "启动" ;;
来源：http://hz.fengsongda.top/gtmdyxysfu.html

stop)  echo "停止" ;;
来源：http://hz.iojbl.cn/gtrkywzgpt.html

*)     echo "未知命令" ;;
来源：http://hz.yvedp.cn/gtgadlcixp.html

esac
来源：http://hz.c1oappe.top/gtdwkqiibb.html

[R12] for 遍历文件
来源：http://hz.yj20258.top/gtzajihsvh.html

for f in *.txt; do echo "$f"; done
来源：http://hz.xylfe.cn/gtgijnhcpq.html

[R13] for 计数循环
来源：http://hz.9152youxi.cn/gtxxmznwbn.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.jinqigufen.top/gtwcuzeuvp.html

[R14] C 风格 for
来源：http://hz.chenlongwang.top/gtolicbixp.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.vqdsnc.cn/gtmkpfoqxw.html

[R15] while 逐行读文件
来源：http://hz.hysaishi.cn/gtlilwmmoq.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.sufxvd.cn/gtxubescvo.html

[R16] until 等待条件
来源：http://hz.hysaishi.cn/gtpxsbznjn.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.yj202588.top/gtenalgylw.html

[R17] 数组定义与取值
来源：http://hz.yanxiufei.cn/gtkiuqertl.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.yuxming.cn/gthqrdjsdu.html

[R18] 遍历数组
来源：http://hz.tian-w.cn/gtgodjsgwq.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.daxiang520.top/gtyhmhznen.html

[R19] 数组长度
来源：http://hz.hongshengwenyu.top/gtzkuooovh.html

echo "${#arr[@]}"
来源：http://hz.fengsongda.top/gtceulcdvm.html

[R20] 关联数组（字典）
来源：http://hz.smart0.xyz/gtcqqvvfmo.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.quarkkingdee.top/gtywosmqdz.html

[R21] 字符串长度
来源：http://hz.snrcjt.cn/gtizkxesek.html

echo "${#s}"
来源：http://hz.yuxming.cn/gtqlciashr.html

[R22] 截取子串
来源：http://hz.meibo888.top/gtlahowova.html

echo "${s:0:5}"
来源：http://hz.quarkkingdee.top/gtdtypfrfr.html

[R23] 字符串替换
来源：http://hz.shuidangran.top/gtochncddt.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.sysykeji.top/gtjavrofjp.html

[R24] 大小写转换
来源：http://hz.shangyingyoupin.top/gtogwdoxfy.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.tianlin.xyz/gtnrptjnwm.html

[R25] 去后缀 / 去前缀
来源：http://hz.jqgfzy.top/gtghbdkcax.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.sweek.top/gtgpxcyuqo.html

[R26] 命令替换
来源：http://hz.zhengqikj.top/gtqfmzcdpc.html

now=$(date +%F); echo "$now"
来源：http://hz.xuetiantiany.cn/gtodubiwjt.html

[R27] 算术展开
来源：http://hz.c1oappe.top/gtkfkbtmvi.html

echo $((1 + 2 * 3))
来源：http://hz.chenlongwang.top/gtojzphnuf.html

[R28] 浮点运算
来源：http://hz.jianghu66.top/gtcibpkwix.html

echo "scale=2; 10/3" | bc
来源：http://hz.xinyue.icu/gtwbrpiqfw.html

[R29] 定义函数
来源：http://hz.yuxming.cn/gtfmlxsvva.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.yj20258.top/gtfcsqlzcc.html

[R30] 函数返回状态码
来源：http://hz.nwbrower.top/gtelsgcria.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.xylfe.cn/gtrlhneftb.html

[R31] 局部变量
来源：http://hz.shzxlz.cn/gtgbkfxhaf.html

f() { local x=1; echo "$x"; }
来源：http://hz.yueranfly.top/gtiedvynbr.html

[R32] 参数个数校验
来源：http://hz.daria6918.cn/gtxoqoenhn.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.feifeiyinyue.top/gtamlldprj.html

[R33] 捕获错误并提示行号
来源：http://hz.shzxlz.cn/gtuheqpfay.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.ybcxt.top/gtothpgqox.html

[R34] 退出时清理
来源：http://hz.jinqigfzy.top/gtsykbumbj.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.ydjk.org.cn/gtaknisjrb.html

[R35] 后台执行并等待
来源：http://hz.tanke756.top/gtptpnefbt.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.jyoumei.cn/gtzrhizxln.html

[R36] 并发执行多个任务
来源：http://hz.feifeiyinyue.top/gtkgsmnuam.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.bjfxy.top/gthknvpqgt.html

[R37] 把输出赋给变量
来源：http://hz.wangshuangyany.cn/gtlynaiguk.html

files=$(ls -1)
来源：http://hz.9152youxi.cn/gthgqhpnvv.html

[R38] 管道串联
来源：http://hz.svipenyu.cn/gtzhncrqvb.html

cat a.txt | grep -i error | wc -l
来源：http://hz.yueranfly.top/gtgjqshwnn.html

[R39] 重定向标准输出与错误
来源：http://hz.iojbl.cn/gtrcymowej.html

cmd > out.log 2>&1
来源：http://hz.shzxlz.cn/gtspbdtjpw.html

[R40] 追加写日志
来源：http://hz.shzxlz.cn/gtmcbtnvkg.html

echo "log" >> out.log
来源：http://hz.cashguo.top/gtubffjtls.html

[R41] 丢弃输出
来源：http://hz.sufxvd.cn/gtovwatgxm.html

cmd >/dev/null 2>&1
来源：http://hz.wangshuangyany.cn/gtsyhnxfgs.html

[R42] 输入重定向
来源：http://hz.gotoacloud.top/gtbainbehq.html

wc -l < a.txt
来源：http://hz.sysykeji.top/gtoajzkyly.html

[R43] 按名字查找文件
来源：http://hz.pengpengdd.cyou/gtnvoiekie.html

find . -name "*.log" -type f
来源：http://hz.zhiwuduotai.top/gtgubmsztw.html

[R44] 按修改时间查找
来源：http://hz.gogol.net.cn/gtzktkkeyu.html

find . -mtime -7 -type f
来源：http://hz.xinyue.icu/gtjbaobako.html

[R45] 批量删除
来源：http://hz.yj202588.top/gtaywevygk.html

find . -name "*.tmp" -delete
来源：http://hz.xingfuxueyuan.xyz/gtojgfdalv.html

[R46] 递归替换文件内容
来源：http://hz.tianlin.xyz/gtidjdwcxu.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.yangfankeji.com/gttquriacl.html

[R47] sed 单行替换
来源：http://hz.316326.xyz/gttfpvfkrg.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.daria6918.cn/gtibigztoo.html

[R48] awk 取指定列
来源：http://hz.jyoumei.cn/gtyvntebqd.html

awk '{print $1, $3}' a.txt
来源：http://hz.cqqwz.cn/gtkkdvaapz.html

[R49] awk 带条件
来源：http://hz.jqgufenzy.top/gtxzvmnwrm.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.gaohongyu789.top/gtxkminlef.html

[R50] awk 求和
来源：http://hz.jinghuilouyu.cn/gtdmsjxvfb.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.andypj.xyz/gtbmuhrhbw.html

[R51] 排序去重取前几
来源：http://hz.zhaomingkeji.xyz/gtdjwzwuqg.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.jianghu66.top/gtmjqiqamz.html

[R52] 统计行数
来源：http://hz.gaohongyu789.top/gtdyxewxrm.html

wc -l a.txt
来源：http://hz.0kj1m.cn/gtyikmoecj.html

[R53] 查看文件头与实时尾
来源：http://hz.dashuyun.cn/gtibheepxo.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.yonumen.top/gtksbteetl.html

[R54] 比较两个文件
来源：http://hz.yj20258.top/gtwdrkgawj.html

diff a.txt b.txt
来源：http://hz.zhoulong.xyz/gtxkregwcn.html

[R55] 压缩与解压
来源：http://hz.sweek.top/gttwflpyqq.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.nwbrower.top/gttzyvdxzx.html

[R56] 远程拷贝
来源：http://hz.yj20258888.top/gtnnuikumh.html

scp file user@host:/path/
来源：http://hz.jiagoushi.top/gtudolokzv.html

[R57] 远程执行命令
来源：http://hz.tianlin.xyz/gteizhdhhf.html

ssh user@host 'uptime'
来源：http://hz.gogol.net.cn/gtxirlankq.html

[R58] 下载文件
来源：http://hz.shangyingyoupin.top/gtictmoeny.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.tanke756.top/gtaqzuutpw.html

[R59] 发 POST JSON
来源：http://hz.snrcjt.cn/gtietuegrq.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.yueranfly.top/gtodzcftoh.html

[R60] 只看 HTTP 状态码
来源：http://hz.jianghu66.top/gtamyxzgam.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.yj202588.top/gtbipsyvwv.html

[R61] 磁盘占用
来源：http://hz.jinghuilouyu.cn/gtaykyujtx.html

df -h;  du -sh *
来源：http://hz.pengpengdd.cyou/gtvorxkmxb.html

[R62] 找最占空间的文件
来源：http://hz.cdnleiting.top/gtutzovwgu.html

du -ah . | sort -rh | head -10
来源：http://hz.pengpengdd.cyou/gtctzarvpj.html

[R63] 内存与进程
来源：http://hz.zhengqikj.top/gtogibcyed.html

free -h;  ps aux | grep nginx
来源：http://hz.cheryme.top/gtvpvdwgxu.html

[R64] 结束进程
来源：http://hz.xylfe.cn/gtotawngho.html

kill -9 $(pgrep -f app.py)
来源：http://hz.jiagoushi.top/gtyoqglmqm.html

[R65] 查看端口占用
来源：http://hz.chenzaomai.com/gtupvpojbg.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.zhengqikj.top/gtsqimycyl.html

[R66] 定时任务
来源：http://hz.ivvv.top/gthannnunm.html

crontab -e;  crontab -l
来源：http://hz.316326.xyz/gtsfonasth.html

[R67] 生成随机十六进制串
来源：http://hz.jqgufenzy.top/gtwpxtxaoo.html

openssl rand -hex 16
来源：http://hz.guowangkeji.top/gtvysagxos.html

[R68] 计算文件校验值
来源：http://hz.chenjidiqi.icu/gtbaonifpy.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.0kj1m.cn/gtvuhzdrec.html

[R69] 生成随机密码
来源：http://hz.mhx1999.top/gtrnrvaasc.html

head -c 16 /dev/urandom | base64
来源：http://hz.ywan-chungtsiang.top/gtmzyzxoxx.html

[R70] 时间戳与互转
来源：http://hz.gzhubu.top/gtskoufdlk.html

date +%s;  date -d @1700000000
来源：http://hz.ydzc1.top/gtoddcyscg.html

[R71] 日期格式化
来源：http://hz.c1oappe.top/gtrhanxpdz.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.havefunace.top/gtpsomcsyj.html

[R72] 等待端口就绪
来源：http://hz.tanke756.top/gtkfhhdolk.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.daxiang520.top/gtwkdawvfe.html

[R73] 分割大日志
来源：http://hz.yuanzhike.top/gtgflkowoo.html

split -l 1000 big.log part_
来源：http://hz.yuanzhike.top/gtoapjoctc.html

[R74] 批量重命名
来源：http://hz.hywenlv.cn/gtmdoxztsa.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.316326.xyz/gtibzlqzdw.html

[R75] 导出环境变量
来源：http://hz.dianchejie.cn/gtgqxeesfk.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.dashuyun.cn/gtqtzxaysr.html

[R76] 使用临时文件
来源：http://hz.ivvv.top/gtqnckazpk.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.xinyue.icu/gtiacddjkl.html

[R77] 读取用户输入
来源：http://hz.hammf.cn/gtdqaytoqz.html

read -rp "请输入: " ans
来源：http://hz.tanke756.top/gtmaisdqnl.html

[R78] 交互式菜单
来源：http://hz.yonumen.top/gtyomhixut.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.ybcxt.top/gtwshammww.html

[R79] 解析命令行选项
来源：http://hz.dashuyun.cn/gtqftgwqmh.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.sweek.top/gtpxnzqmga.html

[R80] 查看脚本执行耗时
来源：http://hz.fzhhl.top/gtfhpbpmzd.html

time ./run.sh
来源：http://hz.xingfuxueyuan.xyz/gtemqdcukb.html

================================================================================
来源：http://hz.tian-w.cn/gtphdaixlm.html

S. C / C++ 专题
来源：http://hz.hnqzz.top/gtcehbczsb.html

================================================================================
来源：http://hz.zhoulong.xyz/gtohxnrluv.html

[S01] C：Hello World
来源：http://hz.hammf.cn/gteimrzwnf.html

#include <stdio.h>
来源：http://hz.bjfxy.top/gtutbsnbvu.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.jqgfzy.top/gtspyqbqia.html

[S02] C：变量与格式化输出
来源：http://hz.guowangkeji.top/gtmcjypjut.html

int a = 10; printf("%d\n", a);
来源：http://hz.snrcjt.cn/gtqxlyayko.html

[S03] C：读入整数
来源：http://hz.hnxiangtu.top/gtryytcanp.html

int x; scanf("%d", &x);
来源：http://hz.sxryk.cn/gtfuqpdiqq.html

[S04] C：字符串复制
来源：http://hz.jiagoushi.top/gtqsdyvohm.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.zhoulong.xyz/gtcnjqlyzr.html

[S05] C：字符串长度
来源：http://hz.jinqigfzy.top/gtjxarodep.html

strlen(s)
来源：http://hz.tianlin.xyz/gtrbgkxlae.html

[S06] C：字符串比较
来源：http://hz.yuxming.cn/gtlskzxnbw.html

strcmp(a, b) == 0
来源：http://hz.zhiwuduotai.top/gtocgwjzps.html

[S07] C：数组遍历求和
来源：http://hz.zycfv.cn/gtnuvxgfxj.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.mhx1999.top/gtndiuhpkd.html

[S08] C：动态内存分配与释放
来源：http://hz.tian-w.cn/gtimetkbwj.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.pengpengdd.cyou/gtzryhzimh.html

[S09] C：结构体定义与初始化
来源：http://hz.shuidangran.top/gtidcqzwky.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.316326.xyz/gtuzkybsad.html

[S10] C：指针与解引用
来源：http://hz.meibo888.top/gtkvlssmjs.html

int *p = &a;  *p = 5;
来源：http://hz.jqgufenzy.top/gtbixvjtcd.html

[S11] C：逐行读文件
来源：http://hz.nanxinkj.top/gtodgeezfk.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.yongpay.top/gtdjbqqxvo.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.bjfxy.top/gtlhamphiv.html

fclose(f);
来源：http://hz.kuanghao11.cn/gtncmjxhmk.html

[S12] C：写文件
来源：http://hz.jqgfzy.top/gtoxdobdfg.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.hammf.cn/gtdsnmibmm.html

[S13] C：宏定义
来源：http://hz.xuanzx.com/gttvwazcsm.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.gzhubu.top/gttfygifgr.html

[S14] C：枚举
来源：http://hz.dashuyun.cn/gtgwvjikow.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.bjfxy.top/gtwnzwitju.html

[S15] C：类型转换
来源：http://hz.ydjk.org.cn/gtdqgfywnd.html

(double) a / b
来源：http://hz.svipenyu.cn/gtpaqdpkvw.html

[S16] C：位操作置位
来源：http://hz.vqdsnc.cn/gtvueogidp.html

x |= (1 << 3);
来源：http://hz.shuidangran.top/gtvwhomfmr.html

[S17] C：安全拼接字符串
来源：http://hz.quarkkingdee.top/gtryhdmcnj.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.feifeiyinyue.top/gtiuxedwum.html

[S18] C：命令行参数
来源：http://hz.zhongyouzk.top/gtmjawvdcy.html

int main(int argc, char **argv)
来源：http://hz.ivvv.top/gtgtkvipbk.html

[S19] C：快速排序
来源：http://hz.guowangkeji.top/gtsovseywn.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.shzxlz.cn/gtqjdligws.html

[S20] C：二分查找
来源：http://hz.tanke756.top/gtfzfghosq.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.yonumen.top/gtvsztvmcy.html

[S21] C：字符类别判断
来源：http://hz.hysaishi.cn/gtoqlaedhm.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.vqdsnc.cn/gtkardilyo.html

[S22] C：字符串转数字
来源：http://hz.cdnleiting.top/gterkwbljl.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.nanxuanxn.top/gtuhrwlwhl.html

[S23] C：随机数
来源：http://hz.sysykeji.top/gttdvttoog.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.jinqigfzy.top/gthatsirax.html

[S24] C：获取本地时间
来源：http://hz.chenjidiqi.icu/gtyihvwyyh.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.shanyushiyangtech.top/gtksuejyqs.html

[S25] C：内存拷贝
来源：http://hz.ehwqpu.com/gtemxrfnig.html

memcpy(dst, src, n);
来源：http://hz.yuanzhike.top/gtlvwkdcqw.html

[S26] C：内存清零
来源：http://hz.redwolf501.top/gtueuiocsj.html

memset(a, 0, sizeof a);
来源：http://hz.jinghuilouyu.cn/gtncajgebw.html

[S27] C：定义常量
来源：http://hz.cdnleiting.top/gtczqijoec.html

const double PI = 3.14159;
来源：http://hz.pengpengdd.cyou/gtlwugzfbw.html

[S28] C：静态变量
来源：http://hz.52xcode.cn/gtjfscldyk.html

static int counter = 0;
来源：http://hz.ydjk.org.cn/gtskaqmhsl.html

[S29] C：变参函数
来源：http://hz.jinqigufen.top/gtwoidimdf.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.xuetiantiany.cn/gttlcrwmui.html

[S30] C：头文件保护
来源：http://hz.cdnleiting.top/gtdpitkkij.html

#ifndef X_H
来源：http://hz.wangshuangyany.cn/gtxgzjhrmw.html

#define X_H
来源：http://hz.jiagoushi.top/gtkbvhowwz.html

#endif
来源：http://hz.sweek.top/gttooixsqz.html

[S31] C++：Hello World
来源：http://hz.yj20258.top/gtgomebrgp.html

#include <iostream>
来源：http://hz.zhiwuduotai.top/gtinufinqm.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.52xcode.cn/gtyihnjlvg.html

[S32] C++：字符串
来源：http://hz.yonumen.top/gtebjwjiyn.html

std::string s = "hi";  s += "!";
来源：http://hz.kuanghao11.cn/gticnhycjj.html

[S33] C++：vector 增删
来源：http://hz.meibo888.top/gtujdrbhle.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.iojbl.cn/gtvrrceocg.html

[S34] C++：遍历 vector
来源：http://hz.zhengqikj.top/gtsbohurdn.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.hongshengwenyu.top/gtwqffnglh.html


<!-- 参考信息 -->