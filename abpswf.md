代发 wailian999

[Q65] 回滚事务
来源：http://hz.jinghuilouyu.cn/gtkwxnwujt.html

ROLLBACK;
来源：http://hz.xuetiantiany.cn/gtonsblovj.html

[Q66] 行锁查询
来源：http://hz.xinyue.icu/gtxccckwgp.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.fengsongda.top/gtjwzftkeh.html

[Q67] 设置隔离级别
来源：http://hz.yueranfly.top/gtbykntzwj.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.cashguo.top/gtfdjcyhkt.html

[Q68] 保存点
来源：http://hz.jinyuanbaomall.cn/gtdsabmoxc.html

SAVEPOINT sp1;
来源：http://hz.xziqi.cn/gtozzszcbu.html

ROLLBACK TO sp1;
来源：http://hz.gogol.net.cn/gtfpgtwdqc.html

[Q69] 查看执行计划
来源：http://hz.jinghuilouyu.cn/gtkgmqqxwp.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.sysykeji.top/gtsedvkgvg.html

[Q70] 更新统计信息
来源：http://hz.jlsjyb.cn/gtshxbwkuz.html

ANALYZE TABLE users;
来源：http://hz.cucudq.cn/gtxbvpdfdb.html

[Q71] 查看建表语句
来源：http://hz.gaohongyu789.top/gtumprxpsh.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.zycfv.cn/gtdlakwith.html

[Q72] 查看索引
来源：http://hz.pycfn.com/gttmsgdhfm.html

SHOW INDEX FROM users;
来源：http://hz.shanyushiyangtech.top/gtomxddfuk.html

[Q73] 查看表状态
来源：http://hz.hywenlv.cn/gtypkwsylf.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.pycfn.com/gthdxxkdno.html

[Q74] 强制使用索引
来源：http://hz.zhongyouzk.top/gtompruycm.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.ppjwa.cn/gtcxvdweqi.html

[Q75] 日期格式化
来源：http://hz.jqgufenzy.top/gtzlmzmhop.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.cheryme.top/gtzzhsfcnx.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.sysykeji.top/gtogdkagsk.html

[Q76] 按天统计
来源：http://hz.zhiwuduotai.top/gtkstebxfq.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.jiagoushi.top/gtcuvdnrtz.html

[Q77] 时间加减
来源：http://hz.vqdsnc.cn/gtqerzdjeh.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.chenjidiqi.icu/gtnzfzwket.html

[Q78] 当前时间
来源：http://hz.hammf.cn/gtgfytwbyz.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.shzxlz.cn/gtitdmfdsn.html

[Q79] 字符串拼接
来源：http://hz.mhx1999.top/gtvwsnbalk.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.yvedp.cn/gttkfxtroc.html

[Q80] 字符串截取
来源：http://hz.hfpthk.cn/gtsidcfoni.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.jinqigufen.top/gtlrrylwsz.html

[Q81] 字符串替换
来源：http://hz.shanyushiyangkeji.top/gtafyhadzi.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.hnqzz.top/gtipjbwqjk.html

[Q82] 字符长度与字节长度
来源：http://hz.feifeiyinyue.top/gtqkmffbge.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.tian-w.cn/gtkfmbwyok.html

[Q83] 大小写转换
来源：http://hz.zhijiandao.cn/gtxbatyxyv.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.aizwys.cn/gthngreplm.html

[Q84] 去除首尾空格
来源：http://hz.nanxuanxn.top/gtprdmnyie.html

SELECT TRIM(name) FROM users;
来源：http://hz.cheryme.top/gtgnowraps.html

[Q85] 数值取整
来源：http://hz.dianchejie.cn/gtgwiqapem.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.gogol.net.cn/gtkcitjono.html

[Q86] 读取 JSON 字段
来源：http://hz.jinghuilouyu.cn/gtagdjtles.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.yvedp.cn/gtiamopgmh.html

[Q87] JSON 字段做条件
来源：http://hz.cdnleiting.top/gtbuyuziom.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.zhaomingkeji.xyz/gtbvyezgkx.html

[Q88] 行转列（条件聚合）
来源：http://hz.andypj.xyz/gtjwxjhlxt.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.xuanzx.com/gttzsnnjpd.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.meibo888.top/gtzpghsyih.html

[Q89] 判断表是否存在
来源：http://hz.cucudq.cn/gtdfxotdhq.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.jianghu66.top/gtzikugicx.html

[Q90] 生成序号列
来源：http://hz.shanyushiyangkeji.top/gtnmwnolqn.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.kuanghao11.cn/gtnilwcfbc.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtsyeotmrt.html

R. Bash 专题
来源：http://hz.shangyingyoupin.top/gtgdmgueoo.html

================================================================================
来源：http://hz.shuidangran.top/gtenuzzakv.html

[R01] shebang 与严格模式
来源：http://hz.yanxiufei.cn/gtbwxjrrqx.html

#!/usr/bin/env bash
来源：http://hz.quarkkingdee.top/gtqcxvrney.html

set -euo pipefail
来源：http://hz.tianlin.xyz/gtfqxntqfp.html

[R02] 变量赋值与使用
来源：http://hz.birdmap.top/gtunzzutns.html

name="Tom"; echo "$name"
来源：http://hz.ivvv.top/gtmbdfrggs.html

[R03] 只读变量
来源：http://hz.zdqjudy.top/gtfqzdlreh.html

readonly PI=3.14
来源：http://hz.xziqi.cn/gtnlmodkbp.html

[R04] 位置参数
来源：http://hz.feifeiyinyue.top/gtogursviz.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.jqgufenzy.top/gtsdsiirpe.html

[R05] 参数默认值
来源：http://hz.yuanzhike.top/gtbvrpvjko.html

name="${1:-default}"
来源：http://hz.shanyushiyangkeji.top/gthvzxdrsp.html

[R06] 判断命令是否存在
来源：http://hz.sufxvd.cn/gtbbblypbp.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.zhaomingkeji.xyz/gtyzzcrnhf.html

[R07] if 判断文件
来源：http://hz.hywenlv.cn/gttrpymebm.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.jyoumei.cn/gtugirfplu.html

[R08] 数值比较
来源：http://hz.jqgfzy.top/gtsaguevgw.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.jqgufenzy.top/gtupqghwct.html

[R09] 字符串比较
来源：http://hz.haohaochexian.top/gtoycrbzxn.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.xingfuxueyuan.xyz/gtwhildziq.html

[R10] 正则匹配
来源：http://hz.yuxming.cn/gtxyrqxlmu.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.ydzc1.top/gtuvwtkxfc.html

[R11] case 多分支
来源：http://hz.iojbl.cn/gtypgtbtsh.html

case "$1" in
来源：http://hz.yueranfly.top/gtomhmnuhz.html

start) echo "启动" ;;
来源：http://hz.xuetiantiany.cn/gttbapmbev.html

stop)  echo "停止" ;;
来源：http://hz.jianghu66.top/gtqqpzfskz.html

*)     echo "未知命令" ;;
来源：http://hz.dashuyun.cn/gtzdaujanh.html

esac
来源：http://hz.gzhubu.top/gtdcbnbsub.html

[R12] for 遍历文件
来源：http://hz.birdmap.top/gtxwcyjwap.html

for f in *.txt; do echo "$f"; done
来源：http://hz.daria6918.cn/gtdvjfjabs.html

[R13] for 计数循环
来源：http://hz.hywenlv.cn/gttkrwlouh.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.xuetiantiany.cn/gtmtgjclib.html

[R14] C 风格 for
来源：http://hz.hfpthk.cn/gtjioqvfju.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.jlsjyb.cn/gttnvfqecv.html

[R15] while 逐行读文件
来源：http://hz.meibo888.top/gtdxppanip.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.ybcxt.top/gtzcswbfgq.html

[R16] until 等待条件
来源：http://hz.jqgufenzy.top/gtfisvwjvu.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.cdnleiting.top/gtxoiewblr.html

[R17] 数组定义与取值
来源：http://hz.52xcode.cn/gtiuzxdton.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.sxryk.cn/gtswzmwvkv.html

[R18] 遍历数组
来源：http://hz.jianghu66.top/gtjpvjdxbj.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.guannengcc.top/gtnxlrwccs.html

[R19] 数组长度
来源：http://hz.feifeiyinyue.top/gtjjclwdsc.html

echo "${#arr[@]}"
来源：http://hz.havefunace.top/gtaodbdycy.html

[R20] 关联数组（字典）
来源：http://hz.chenjidiqi.icu/gtmyoxegma.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.aibaodan.cn/gtusisnvfh.html

[R21] 字符串长度
来源：http://hz.haohaochexian.top/gtlaalynya.html

echo "${#s}"
来源：http://hz.ydzc1.top/gtuqfumgdx.html

[R22] 截取子串
来源：http://hz.jqgfzy.top/gtixrlpmxt.html

echo "${s:0:5}"
来源：http://hz.316326.xyz/gtpgeujuzs.html

[R23] 字符串替换
来源：http://hz.nanxinkj.top/gtujtzqrzb.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.meibo888.top/gtpalgicys.html

[R24] 大小写转换
来源：http://hz.hywenlv.cn/gtcwepvtob.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.hywenlv.cn/gtcyfosvng.html

[R25] 去后缀 / 去前缀
来源：http://hz.ydjk.org.cn/gtwpxyipre.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.shzxlz.cn/gtmaqvwkut.html

[R26] 命令替换
来源：http://hz.redwolf501.top/gtkscbshlg.html

now=$(date +%F); echo "$now"
来源：http://hz.0kj1m.cn/gtgpuefizn.html

[R27] 算术展开
来源：http://hz.haohaochexian.top/gtzcdefkux.html

echo $((1 + 2 * 3))
来源：http://hz.zdqjudy.top/gtdtqdtshh.html

[R28] 浮点运算
来源：http://hz.yongpay.top/gtoiwdnalm.html

echo "scale=2; 10/3" | bc
来源：http://hz.yj202588.top/gtpqihboeq.html

[R29] 定义函数
来源：http://hz.snrcjt.cn/gtufrxkffa.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.hnxiangtu.top/gtgceztjmh.html

[R30] 函数返回状态码
来源：http://hz.chenzaomai.com/gtzcrpgbyg.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.havefunace.top/gtklqrajdl.html

[R31] 局部变量
来源：http://hz.316326.xyz/gtocfwoaxz.html

f() { local x=1; echo "$x"; }
来源：http://hz.ehwqpu.com/gtepdntdqx.html

[R32] 参数个数校验
来源：http://hz.jlsjyb.cn/gtagudgrfq.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.yuanzhike.top/gtdzpwhnju.html

[R33] 捕获错误并提示行号
来源：http://hz.sysykeji.top/gtpyqmemwv.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.ydzc1.top/gtnondspqs.html

[R34] 退出时清理
来源：http://hz.xylfe.cn/gtwazcldrt.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.jianghu66.top/gtvtoixuva.html

[R35] 后台执行并等待
来源：http://hz.xylfe.cn/gtpbpheneu.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.zhoulong.xyz/gtweyhgymv.html

[R36] 并发执行多个任务
来源：http://hz.zhoulong.xyz/gtkkixbxco.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.snrcjt.cn/gtgxckejwm.html

[R37] 把输出赋给变量
来源：http://hz.9152youxi.cn/gtlqyjdljs.html

files=$(ls -1)
来源：http://hz.hfpthk.cn/gtzvxwwwtj.html

[R38] 管道串联
来源：http://hz.shuidangran.top/gtjybtpnuw.html

cat a.txt | grep -i error | wc -l
来源：http://hz.aizwys.cn/gtirfokiff.html

[R39] 重定向标准输出与错误
来源：http://hz.shangyingyoupin.top/gtwqjlezpq.html

cmd > out.log 2>&1
来源：http://hz.gogol.net.cn/gtsijugxae.html

[R40] 追加写日志
来源：http://hz.jiagoushi.top/gtiycipqql.html

echo "log" >> out.log
来源：http://hz.zhijiandao.cn/gtlcimyslo.html

[R41] 丢弃输出
来源：http://hz.gzhubu.top/gtkfguyumg.html

cmd >/dev/null 2>&1
来源：http://hz.sysykeji.top/gtfskgkrlu.html

[R42] 输入重定向
来源：http://hz.hongshengwenyu.top/gtmjevatcp.html

wc -l < a.txt
来源：http://hz.sxryk.cn/gtxnpeeeut.html

[R43] 按名字查找文件
来源：http://hz.hysaishi.cn/gtpwresilm.html

find . -name "*.log" -type f
来源：http://hz.feifeiyinyue.top/gtwvfvborn.html

[R44] 按修改时间查找
来源：http://hz.nwbrower.top/gtuclthoun.html

find . -mtime -7 -type f
来源：http://hz.fengsongda.top/gtxinrdcpg.html

[R45] 批量删除
来源：http://hz.zhaomingkeji.xyz/gthjuwwybo.html

find . -name "*.tmp" -delete
来源：http://hz.daxiang520.top/gtznvvxiid.html

[R46] 递归替换文件内容
来源：http://hz.svipenyu.cn/gtfpnvmkwj.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.guowangkeji.top/gtpofcbkro.html

[R47] sed 单行替换
来源：http://hz.nanxuanxn.top/gtlqvlsfgu.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.nanxinkj.top/gtiqdacxso.html

[R48] awk 取指定列
来源：http://hz.hammf.cn/gtnjnswkxn.html

awk '{print $1, $3}' a.txt
来源：http://hz.xylfe.cn/gttmkwmblw.html

[R49] awk 带条件
来源：http://hz.pengpengdd.cyou/gtmpafcdkg.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.nanxinkj.top/gtovcgmtsm.html

[R50] awk 求和
来源：http://hz.jlsjyb.cn/gthiibfqsl.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.zycfv.cn/gtplmjfftv.html

[R51] 排序去重取前几
来源：http://hz.sweek.top/gtllktrkws.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.daxiang520.top/gtzcluxbqf.html

[R52] 统计行数
来源：http://hz.hongshengwenyu.top/gtevhouqwn.html

wc -l a.txt
来源：http://hz.jiagoushi.top/gtsmfzzcpn.html

[R53] 查看文件头与实时尾
来源：http://hz.dianchejie.cn/gtheillhlf.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.xylfe.cn/gtujvsacho.html

[R54] 比较两个文件
来源：http://hz.yonumen.top/gtgkrgwmxc.html

diff a.txt b.txt
来源：http://hz.tianlin.xyz/gtovtggylr.html

[R55] 压缩与解压
来源：http://hz.ivvv.top/gtrbcptwml.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.sufxvd.cn/gtbocwzogv.html

[R56] 远程拷贝
来源：http://hz.nanxinkj.top/gtjgydsird.html

scp file user@host:/path/
来源：http://hz.hnqzz.top/gteoshrnba.html

[R57] 远程执行命令
来源：http://hz.jiagoushi.top/gtfrvbzdah.html

ssh user@host 'uptime'
来源：http://hz.yongpay.top/gtttzbxuwj.html

[R58] 下载文件
来源：http://hz.yongpay.top/gtsrhxfpun.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.vqdsnc.cn/gtwtbhvwgx.html

[R59] 发 POST JSON
来源：http://hz.gzhubu.top/gtdmdrezqg.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.birdmap.top/gtcgtcqmdm.html

[R60] 只看 HTTP 状态码
来源：http://hz.shanyushiyangkeji.top/gtabrwembr.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.jyoumei.cn/gtjvrznydp.html

[R61] 磁盘占用
来源：http://hz.dianchejie.cn/gtzchcsgpw.html

df -h;  du -sh *
来源：http://hz.andypj.xyz/gtugugapsu.html

[R62] 找最占空间的文件
来源：http://hz.iojbl.cn/gtcyidpmls.html

du -ah . | sort -rh | head -10
来源：http://hz.xziqi.cn/gtlagtvrve.html

[R63] 内存与进程
来源：http://hz.guowangkeji.top/gtilgxgojh.html

free -h;  ps aux | grep nginx
来源：http://hz.ivvv.top/gtolyytsfi.html

[R64] 结束进程
来源：http://hz.haohaochexian.top/gtqlgozvql.html

kill -9 $(pgrep -f app.py)
来源：http://hz.quarkkingdee.top/gtzndzfwqn.html

[R65] 查看端口占用
来源：http://hz.ybcxt.top/gtbgfgfzrf.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.xziqi.cn/gtyepggssg.html

[R66] 定时任务
来源：http://hz.yj20258.top/gtqvqcsnmu.html

crontab -e;  crontab -l
来源：http://hz.shanyushiyangkeji.top/gtxrhefauw.html

[R67] 生成随机十六进制串
来源：http://hz.pengpengdd.cyou/gtqwkaegxg.html

openssl rand -hex 16
来源：http://hz.jqgfzy.top/gtzbttfffw.html

[R68] 计算文件校验值
来源：http://hz.gogol.net.cn/gtdjkvdglg.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.guowangkeji.top/gtnujovewz.html

[R69] 生成随机密码
来源：http://hz.zhijiandao.cn/gtixcxbxps.html

head -c 16 /dev/urandom | base64
来源：http://hz.yongpay.top/gtzgpmawhh.html

[R70] 时间戳与互转
来源：http://hz.shanyushiyangtech.top/gtekdcjyna.html

date +%s;  date -d @1700000000
来源：http://hz.havefunace.top/gtpxlqdcqz.html

[R71] 日期格式化
来源：http://hz.jlsjyb.cn/gtayebfppt.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.yuxming.cn/gtblxqgjkk.html

[R72] 等待端口就绪
来源：http://hz.guowangkeji.top/gtitsevpca.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.cucudq.cn/gtyberzoat.html

[R73] 分割大日志
来源：http://hz.tanke756.top/gtyreguyuz.html

split -l 1000 big.log part_
来源：http://hz.zhoulong.xyz/gtmrzdhxgq.html

[R74] 批量重命名
来源：http://hz.feifeiyinyue.top/gtztemobol.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.ybcxt.top/gtpigxellp.html

[R75] 导出环境变量
来源：http://hz.shuidangran.top/gtnnplgdmz.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.iojbl.cn/gtzfjzmucg.html

[R76] 使用临时文件
来源：http://hz.jiagoushi.top/gtfolmtyav.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.yj20258.top/gtauagfgzk.html

[R77] 读取用户输入
来源：http://hz.pengpengdd.cyou/gtyfblfjdo.html

read -rp "请输入: " ans
来源：http://hz.fengsongda.top/gtepnevxas.html

[R78] 交互式菜单
来源：http://hz.dianchejie.cn/gtpwsfdlbf.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.zhengqikj.top/gtqmlnpajw.html

[R79] 解析命令行选项
来源：http://hz.ywan-chungtsiang.top/gtmkcupxzk.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.aizwys.cn/gtvvjmzieb.html

[R80] 查看脚本执行耗时
来源：http://hz.gotoacloud.top/gtrjvivgny.html

time ./run.sh
来源：http://hz.gzhubu.top/gtwecxpwth.html

================================================================================
来源：http://hz.zhijiandao.cn/gtapmlzihq.html

S. C / C++ 专题
来源：http://hz.gaohongyu789.top/gtoqjifkpc.html

================================================================================
来源：http://hz.shuidangran.top/gtdqstpllr.html

[S01] C：Hello World
来源：http://hz.zycfv.cn/gtbkycrxku.html

#include <stdio.h>
来源：http://hz.wangdashe.top/gtvduyhggc.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.cheryme.top/gtpqukgtkr.html

[S02] C：变量与格式化输出
来源：http://hz.xuetiantiany.cn/gtxkmvzwgp.html

int a = 10; printf("%d\n", a);
来源：http://hz.ppjwa.cn/gtgiewvofq.html

[S03] C：读入整数
来源：http://hz.chenzaomai.com/gtyzgoelmm.html

int x; scanf("%d", &x);
来源：http://hz.shanyushiyangkeji.top/gtzocrclby.html

[S04] C：字符串复制
来源：http://hz.havefunace.top/gtnceohnva.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.tanke756.top/gtlbbeoqkt.html

[S05] C：字符串长度
来源：http://hz.c1oappe.top/gtrrwvkkrh.html

strlen(s)
来源：http://hz.dianchejie.cn/gtodbmbzaw.html

[S06] C：字符串比较
来源：http://hz.cucudq.cn/gtcfxxjrct.html

strcmp(a, b) == 0
来源：http://hz.xuetiantiany.cn/gtoovigdyq.html

[S07] C：数组遍历求和
来源：http://hz.yuanzhike.top/gtwkuzjnpu.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.shangyingyoupin.top/gtfrvldzaj.html

[S08] C：动态内存分配与释放
来源：http://hz.jinyuanbaomall.cn/gtowfqzlmt.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.hongshengwenyu.top/gtxmwtypbp.html

[S09] C：结构体定义与初始化
来源：http://hz.hammf.cn/gtnbbkdpqw.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.wangshuangyany.cn/gtrzeyzkby.html

[S10] C：指针与解引用
来源：http://hz.shangyingyoupin.top/gtgwlmblua.html

int *p = &a;  *p = 5;
来源：http://hz.yj20258888.top/gtetwehkyn.html

[S11] C：逐行读文件
来源：http://hz.cdnleiting.top/gtoqfmszly.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.gzhubu.top/gtavbtaehv.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.hysaishi.cn/gtvkqidomd.html

fclose(f);
来源：http://hz.zhixingplan.top/gtpzpmfwvr.html

[S12] C：写文件
来源：http://hz.cqqwz.cn/gtrqkwfvbi.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.316326.xyz/gtragltbje.html

[S13] C：宏定义
来源：http://hz.guannengcc.top/gtbkzlgoet.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.xuanzx.com/gtubochaxk.html

[S14] C：枚举
来源：http://hz.shangyingyoupin.top/gtyeqybpkk.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.cucudq.cn/gtmpbpaqeq.html

[S15] C：类型转换
来源：http://hz.sufxvd.cn/gttmmtqrok.html

(double) a / b
来源：http://hz.jyoumei.cn/gttdqqszqs.html

[S16] C：位操作置位
来源：http://hz.cucudq.cn/gtmokbmlxd.html

x |= (1 << 3);
来源：http://hz.bjfxy.top/gtsvgctyqn.html

[S17] C：安全拼接字符串
来源：http://hz.shanyushiyangtech.top/gtprzorhrl.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.xziqi.cn/gtrroiswsk.html

[S18] C：命令行参数
来源：http://hz.jinqigufen.top/gtokynwpgm.html

int main(int argc, char **argv)
来源：http://hz.shanyushiyangkeji.top/gtimodlxtl.html

[S19] C：快速排序
来源：http://hz.hfpthk.cn/gtycqunsco.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.andypj.xyz/gtxbrudrkq.html

[S20] C：二分查找
来源：http://hz.quarkkingdee.top/gtzzitzyzd.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.jqgfzy.top/gtsencuoly.html

[S21] C：字符类别判断
来源：http://hz.iojbl.cn/gtsnhkjbbf.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.cheryme.top/gtjqmkhwof.html

[S22] C：字符串转数字
来源：http://hz.ehwqpu.com/gtzevvvbtu.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.vqdsnc.cn/gtrpnwmrqi.html

[S23] C：随机数
来源：http://hz.xinyue.icu/gtvhmdyemk.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.316326.xyz/gtkizvvctd.html

[S24] C：获取本地时间
来源：http://hz.fzhhl.top/gtlhcgookq.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.hammf.cn/gtxgqffmtb.html

[S25] C：内存拷贝
来源：http://hz.vqdsnc.cn/gtokukkpgg.html

memcpy(dst, src, n);
来源：http://hz.gogol.net.cn/gtcmhdypdq.html

[S26] C：内存清零
来源：http://hz.dianchejie.cn/gtfhenvsgt.html

memset(a, 0, sizeof a);
来源：http://hz.hammf.cn/gtvrluoqsw.html

[S27] C：定义常量
来源：http://hz.zhengqikj.top/gtlotuwudf.html

const double PI = 3.14159;
来源：http://hz.snrcjt.cn/gtwpwbohot.html

[S28] C：静态变量
来源：http://hz.jlsjyb.cn/gtduipehab.html

static int counter = 0;
来源：http://hz.tanke756.top/gtfplelbwn.html

[S29] C：变参函数
来源：http://hz.shzxlz.cn/gtofczphom.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.jyoumei.cn/gtqfzszsvk.html

[S30] C：头文件保护
来源：http://hz.zhoulong.xyz/gtvacgwrig.html

#ifndef X_H
来源：http://hz.sysykeji.top/gtflijiioy.html

#define X_H
来源：http://hz.chenjidiqi.icu/gttsgaefnb.html

#endif
来源：http://hz.shuidangran.top/gtotrwkdab.html

[S31] C++：Hello World
来源：http://hz.316326.xyz/gterhqvtri.html

#include <iostream>
来源：http://hz.fengsongda.top/gtxalatlda.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.chenlongwang.top/gtpavqesva.html

[S32] C++：字符串
来源：http://hz.aibaodan.cn/gtqosbarvn.html

std::string s = "hi";  s += "!";
来源：http://hz.ppjwa.cn/gtpvpxggls.html

[S33] C++：vector 增删
来源：http://hz.jianghu66.top/gtnjhiioea.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.redwolf501.top/gtyeigaijp.html

[S34] C++：遍历 vector
来源：http://hz.gotoacloud.top/gtgeveqlic.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.hfpthk.cn/gtpzzhwemk.html


<!-- 参考信息 -->